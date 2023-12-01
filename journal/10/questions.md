# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | It organizes code into logical groups  |

02. What is the difference between a `class` and an `interface`?

  > |  a class describes the behavior of an object, an interface contains the behavior defined and assigned by the class |

03. What is the method that returns an instance of a class, yet it has no return type?

  > | the void method |

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > | It is public. |

06. In the Car example what is `string` an indication of?

  > |It is the data type.|

07. In the Car example what is `abstract` preventing?

  > |It prevents users from using any other class hierarchy. |

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | columns are vertical information and describe the information, and hold a list of named values from the same field. rows are horizontal information in the table, and are the actual value.  |

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > |CREATE TABLE IN CHARATERS
> id INT NOT NULL PRIMARY KEY AUTO_INCREMENT COMMENTS "this is the id of the character"
> name CHAR(255) NOT NULL COMMENTS "this is the name of the character"
> age INT NOT NULL COMMENTS "this is the age of the character"
> description CHAR(255) NOT NULL COMMENTS "this is the description of the character"
> |

10. In SQL how can you query more than a single table? Provide an example.

  > |We use the join operator, which joins the tables together. We say SELECT ing.*, acc.* FROM ingredients ing JOIN accounts acc ON acc.id = ing.creatorId WHERE ing.id = LAST_INSERT_ID();";|
