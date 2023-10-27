# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > |An entrypoint is what identifies the resource that is an access point to the application |

02. What is the difference between a vue `component` and `page`?

  > | the vue compenent is a reusable instance with custom HTML elements, the page is the main compenent to display and operate content |

03. What is ***Component-Based Architecture***?

  > | It is a framework for building software based on reusable components|

04. What are the three tags that make up a Vue component?

  > | template, script, and style.  |

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > |Lifecycle hooks are a window into how the library you are using really works. They allow you to know when your component is created, addded, updated, and destroyed. They provide a specified amount of time to complete an action before that action transitions to the next state.|

06. Which component in Vue does the vue-router use to mount pages onto?

  > |the navbar.vue component |

07. What is the difference between the `AppState` and the state object within a component?

  > | The appstate is global, and the component state is local|

08. What is the responsibility of `Services` in our Vue projects?

  > |they act as pieces of reuasable and testable code that you can use all across your application, they work similarily to the services in the MVC template |

09. What are ***props*** and how are they used? Provide an example

  > | they are custom attributes that we register on our Vue projects. They are used to pass data from a parent to child component. For example we have a template tag with CAMERA in it. We use prop tags such as image and name to define that camera. We use the :v-bind on this. 

10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > | Watchers, or calling the watch function |
