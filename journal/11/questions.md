# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | It enables us to create new classes that reuse, extend, and modify the behavior defined in other classes.  |

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > |The class whose members are inherited is called the base class,  and the class that inherits those members is called the derived class. Yes, it does inherit all those classes.  |

3. How does ***accessibility*** affect inheritance?

  > |A members accessibility affects its visibitilty for a derived class.  |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | A primary key is a unique identifier for each record on the table. A foreign key establishes a relationship between tables by referencing the primary key of another table.  |

5. What is an ***alias***?

  > |We specify a class name using its fully qualified namespace. Then we can use that name within the scope. |

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > | string sql = @"SELECT pat.*,
> doc.*,
> acc.*
> FROM patients pat
> JOIN doctors doc ON pat.doctorId = doc.id
> JOIN accounts acc ON acc.id = doc.creatorId
> WHERE pat.accountId = @userId;";
> List <Patient> patient = _db.Query<Patient, Account, Patient> (sql, (patient, account)
=> {
> patient.Creator = account
> return patient
> }, new {userId}) .ToList();
> return patient 
> 
> |
