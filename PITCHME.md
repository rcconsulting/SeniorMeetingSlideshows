## Global Config
A technique for managing your state- and configuration-related global values.
+++
### Steve Allen
- github.com/steveAllen0112
- steven.allen@rcconsulting.com
---

### Historical Methods

@box[bg-orange text-white box-padding fragment](Global Fields)
@box[bg-orange text-white box-padding fragment](Session Records)
@box[bg-orange text-white box-padding fragment](Global Variables (Vanilla))

---

@snap[north span-100]
### Global Fields
@snapend

@snap[west span-45]
#### Pros:
@box[bg-green text-white box-padding fragment](Can maintain state on a local file.)
@box[bg-green text-white box-padding fragment](Useful for Container UI.)
@snapend

@snap[east span-45]
#### Cons:
@box[bg-orange text-white box-padding fragment](Clutter up your database)
@snapend

---

@snap[north span-100]
### Session Records
@snapend

@snap[west span-45]
#### Pros:
@box[bg-green text-white box-padding fragment](Can maintain state even on a served file.)
@snapend

@snap[east span-45]
#### Cons:
@box[bg-orange text-white box-padding fragment](Record-based, and therefore contextual.)
@box[bg-orange text-white box-padding fragment](Still take up room in the Database.)
@snapend

---

@snap[north span-100]
### Global Variables
@snapend

@snap[west span-45]
#### Pros:
@box[bg-green text-white box-padding fragment](Can be inspected and updated all in one place.)
@box[bg-green text-white box-padding fragment](No schema clutter!)
@box[bg-green text-white box-padding fragment](Self-cleaning, even on local files!)
@snapend

@snap[east span-45]
#### Cons:
@box[bg-orange text-white box-padding fragment](Not really portable easily.)
@box[bg-orange text-white box-padding fragment](Are absolutely individual things.)
@box[bg-orange text-white box-padding fragment](Must rely on memory of strict naming and namespacing rules)
@box[bg-orange text-white box-padding fragment](Rules are not well-defined unless the developer makes them so)
@snapend

---

### A New Tool: Global Config

With the advent of several changes in recent versions, a specific variation on the Global Variables general technique becomes attractive: Global Configuration.

@ul

 - Custom Functions for everyone
 - Native JSON

@ulend

---

### A New Tool: Global Config

@box[bg-green text-white box-padding fragment](Concept: Pack all your global state and configuration data into one data object stored in _one_ global variable.)

@box[bg-pink box-padding fragment](Data Object: JSON)
@box[bg-pink box-padding fragment](Ease of Use: Custom Functions)

---

### Use Cases

@box[bg-green text-white box-padding fragment](Save & Restore State#If you need to quickly save the entire state data all at once.)

@box[bg-green text-white box-padding fragment](Debug Report#Often you don't have a long time!)

@box[bg-green text-white box-badding fragment](Developer Efficiency#You don't have to remember everything. It's all there!)