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
@ol
- Can maintain state on a local file.
- Useful for Container UI.
@olend
@snapend

@snap[east span-33]
#### Cons:
@ol
- Clutter up your database
@olend
@snapend

---
@snap[north span-100]
### Session Records
@snapend

@snap[east span-33]
#### Pros:
@ol
- Can maintain state even on a served file.
@olend
@snapend

@snap[west span-33]
#### Cons:
@ol
- Record-based, and therefore contextual.
  @ul
  -There are some workarounds to this.
  @ulend
- Still take up room in the Database.
@olend
@snapend

---

@snap[north span-100]
### Global Variables
@snapend

@snap[west span-33]
#### Pros:
@ol
- Can be inspected and updated all in one place.
  @ul
  - (Data Viewer)
  @ulend
- No schema clutter!
- Self-cleaning, even on local files!
  @ul
  - (unlike Global Fields)
  @ulend
@olend
@snapend

@snap[east span-33]
#### Cons:
@ol
- Not really portable easily.
- Are absolutely individual things.
  @ul
  - (Must rely on memory of strict naming and namespacing rules)
  - (Rules are not well-defined unless the developer makes them so)
  @ulend
@olend
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
