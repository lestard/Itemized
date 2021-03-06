# Requirements

The intent of the project *Itemized* is to provide a system that allows the user to freely structure items of data.


## The name Itemized

The name of the project is *Itemized* which has the word item in it. The word item has a very unspecific character and simply describes a thing that might belong to any set of things. Simplictiy and freedom is exactly the purpose this project has. 

The name was inspired by the Latex typesetting system. Latex provides a command `\itemize` which is used to start a listing of items.  

## Use Cases

When we started the project we had multiple use cases in mind that could be solved by such a system. To give you an idea of what we have in mind we describe some of these use cases here in more detail.

### Task management system.

Task management systems are used to plan and manage tasks that you have to work on. For example in software development it's a common practice to keep track of tasks that are needed to be done to create a new feature. 

There are lots of task mangements systems available that are naming their items *Issues*, *Tasks*, *Workitems* or *Bugs* or similar terms. Most of the task management systems are very specific for a domain or force the user to fit his ideas into their constrainted structures. Often the user then needs to hack the constraints and structures to still express his ideas in those systems.

One specific example: There may be a system that structures its items in a parent child relationship where the parent is some kind of a container type and the child is some kind of element in that container and the child itself cannot have any children. To build a more complex tree structure with those items the user has to use other ways to express that natural relationship. He maybe puts a link to the next child item into the content of the created child. Another problem of this very closed structure is that a child item can only have one parent item. If the user wants to express that an idea (item) has two or more causes (items) than he again has to find another hack for this purpose.

So in the context of this projects ideas should be freely composable and easily managable. An item can express any idea and also be connected to any other idea like human thoughts do.

## Freedom to structure items

To freely structure items with a specific idea in mind it is natural that the user should be allowed to connect as many items with each other as he likes. The meaning of the structure and the relations should be defined by the user. If this process of composing shall be so easy so the user doesn't need to known many rules it must not follow to many constraints.

The following points make that explanation more specific:

* Items have some kind of content: A title, a description, an amount of attachments (multimedia).
* Items can have a relationship to others. Their relationship has no predefined and fixed meaning. It shall be defined by the user. For that purpose some kind of label will serve.
* Items can have a state but they don't need to. This state should also be defined by the user using labels. If an 
item should have a task character then it may have a label "open", "in progress" or "done".
* Items belong to some kind of context. Each item has a context and some can share the same context. For example a context can be a project.
* Items have a unique id that allows easy sharing of them. This will be easy when the item id is an URI.

## Conditional Constraints

Although the nature of this project shall be free and as little limiting as possible sometimes constraints are desired. But this is a condition the user has to define. That is the user should be able to request the system to guarantee that specific constraints are met. The user may want to define specific labels for states and wants to ensure that only these states are used for his items. This feature may be desirable when the system is used collaboratively. So many users try to create items and try to use their own labels. But under certain conditions it might be desirable to avoid that.
