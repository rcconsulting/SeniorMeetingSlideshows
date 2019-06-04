## Global Config
A technique for managing your state- and configuration-related global values.
+++
### Steve Allen
- github.com/steveAllen0112
- steven.allen@rcconsulting.com
---

### Historical Methods

@box[fragment](Global Fields)
@box[fragment](Session Records)
@box[fragment](Global Variables (Vanilla))

---

@snap[north span-100]
### Global Fields
@snapend

@snap[west span-33]
#### Pros:
@box[fragment](Can maintain state on a local file.)
@box[fragment](Useful for Container UI.)
@snapend

@snap[east span-33]
#### Cons:
@box[fragment](Clutter up your database)
@snapend

---

@snap[north span-100]
### Session Records
@snapend

@snap[east span-33]
#### Pros:
@box[fragment](Can maintain state even on a served file.)
@snapend

@snap[west span-33]
#### Cons:
@box[fragment](Record-based, and therefore contextual.)
@box[fragment](Still take up room in the Database.)
@snapend

---

@snap[north span-100]
### Global Variables
@snapend

@snap[west span-33]
#### Pros:
@box[fragment](Can be inspected and updated all in one place.)
@box[fragment](No schema clutter!)
@box[fragment](Self-cleaning, even on local files!)
@snapend

@snap[east span-33]
#### Cons:
@box[fragment](Not really portable easily.)
@box[fragment](Are absolutely individual things.)
@box[fragment](Must rely on memory of strict naming and namespacing rules)
@box[fragment](Rules are not well-defined unless the developer makes them so)
@snapend

---

### A New Tool: Global Config

@box(With the advent of several changes in recent versions, a specific variation on the Global Variables general technique becomes attractive: Global Configuration.)

@ul

 - Custom Functions for everyone
 - Native JSON

@ulend

---

### A New Tool: Global Config

@box[fragment](Concept: Pack all your global state and configuration data into one data object stored in _one_ global variable.)

@box[fragment](Data Object: JSON)
@box[fragment](Ease of Use: Custom Functions)
