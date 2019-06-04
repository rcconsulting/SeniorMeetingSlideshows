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

+++

### Global Fields
#### Pros:
@ol
- Can maintain state on a local file.
- Useful for Container UI.
@olend

#### Cons:
@ol
- Clutter up your database
@olend

+++

### Session Records
#### Pros:
@ol
- Can maintain state even on a served file.
@olend

#### Cons:
@ol
- Record-based, and therefore contextual.
  @box[fragment] There are some workarounds to this.
- Still take up room in the Database.
@olend

+++
### Global Variables
#### Pros:
@ol
- Can be inspected and updated all in one place.
  @box[fragment](Data Viewer)
- No schema clutter!
- Self-cleaning, even on local files!
  @box[fragment](unlike Global Fields)
@olend

#### Cons:
@ol
- Not really portable easily.
- Are absolutely individual things.
  @box[fragment](Must rely on memory of strict naming and namespacing rules)
  @box[fragment](Rules are not well-defined unless the developer makes them so)
@olend

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
