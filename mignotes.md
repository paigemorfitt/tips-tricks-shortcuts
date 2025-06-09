## Islandora Metadata Interest Group Agenda
### Monday, August 12, 2024, [1-2pm EDT](http://www.thetimezoneconverter.com/?t=1%20pm&tz=Toronto&) 
#### Join Us Virtually!
* Zoom Link: https://us02web.zoom.us/j/93923574947?pwd=Z1kyY01veFJNbFZFVUg4Mm1jS1FyZz09

---
## Chair Roster
* Chris Day 🤿
* Rosie Le Faive 🪑
* Paige Morfitt  📝
---

#### Working Documents:
* [Islandora Starter Site Metadata Configuration](https://docs.google.com/spreadsheets/d/1N37GSwiDl_DSH9-n3BhWLUtjZohOg2udGJJlnZ8BmWQ/edit#gid=0)
* [Islandora Starter Site Metadata Documentation](https://islandora.github.io/documentation/user-documentation/starter-site-metadata-configuration/)
* [CLAW MIG MODS simplified mapping](https://docs.google.com/spreadsheets/d/18u2qFJ014IIxlVpM3JXfDEFccwBZcoFsjbBGpvL0jJI/edit#gid=0)
* [Example MODS for CLAW mapping](https://docs.google.com/spreadsheets/d/1C2Xie7HUDSgRT5v4ldoJvlNdoXz2GHAPvL3PE3TOKW8/edit#gid=1829081124)
* [Draft Recommendations](https://docs.google.com/document/d/15qSO9YcALtYSqd6CUuGx0t8FwUJ5pPwVPz0PA5rU898/edit#heading=h.f9r6knw0rjvu)
* [Feedback on Mapping from ICG, Part 2](https://docs.google.com/document/d/11OpqMMCXM1TFXgsr4yyTQ_cH9DabnD31p7JnuTRQl28/edit?invite=CMWvruEI&ts=5e66437f)
* [Wants/Needs/Questions Open Document](https://docs.google.com/document/d/12Kpb6826TNPzzMuyPS0sESa9TLnmljQmeioWbaPeEdA/edit)
* [Working Ideas](https://github.com/islandora-interest-groups/Islandora-Metadata-Interest-Group/blob/main/working_docs/ideas_and_topics.md)
* [MIG I8 Glossary](https://docs.google.com/document/d/1cfPYFVV9qvvz2VjBRdYUN0CB7AyVDuG-GYavQ27DuBk/edit#heading=h.9fr9xw70meix)

---

#### Attending:
* Rosie
* Paige
* Tyrica Terry Kapral
* Tracy Tolf
* Dani Kroon
* Mike Bolam
* Meaghan Else Cash
* Seth Shaw
* Ann Marie Mesco
* Kara Hart


### Agenda: 
* Announcements
* Changes to Starter Site
* Revisions by Default on Taxonomy Terms
* Typed Relation With Display Name
* Equations in Abstract
* Title - priorities?
* Open Discussion
* Glossary Review

### Notes:
* DrupalCon in Barcelona. 
* No changes. Nothing that will impact any metadata
* Taxonomy Terms: Turning on revisions by default
    * In Drupal, they created a way to make revisions in metadata terms
    * Question: Do we want to turn this on by default on all/any of our vocabularies? 
        	* Go to genre taxonomy, select a term, and click "revisions".
        	* Automatically the content will show the new name. 
        	* You click the 'revisions' tab, it will show you when the term was revised. It also allows you to revert the term back. The revert puts the old value back in addition to the new value (it does not rewind or rewrite). 
    	* Question: What does the revision do? 
         *  A log of changes to taxonomy terms. It is useful to see, however you do need to do some digging to see what has been changed. But it would keep us  honest and be available for auditing/for quality control if you have a student change terms you can check their revisions. It does take more space in the database. People already have the ability to do this, but it's about making it a default. 
    	* You don't have to do it for every taxonomy either. 
    	* This would only be if the taxonomy terms changes, but changing the data on the object wouldn't change anything. This would only track the taxonomy term change (so if you move something embargoed out of embargoed, it would not be tracked). 
    	* when you change a person's name in the taxonomy, you have in theory changed the metadata in all the records that use that term. the node doesn't know that
    	* It would be helpful to look at our metadata as a series of links. 
    * Rosie will put up a pull request to default making revisions on taxonomies

Typed Relation With Display Name
* Rosie made a thing. 
* Rosie made a Display Name field in Typed Relation 
* So if you have a name, but the name has been changed or you want to display something in a more human-readable form (example, Lastname,FirstName (YYYY- ) but you want FirstName LastName)
* The display name is optional. If you don't use it, it will default to the field. 
* This is a way to associate a name with a person at the time. if you want to bulk change it does make it a bit more challenging, but its no more challenging than other bulk changing. 
* if you want to adapt this to your site, you cannot change the type of field easily. you need to make a new field, export data (workbench) reimport that data via workbench, and set up your facets and all that. 
* Interest in this in place of contributors typed relation field? workbench integration is important. rosie hasn't done all the tests yet. 
* to put into your workbench: 
	relators:aut:person:Rosie Le Faive~Lefaive,R
	where everything after ~ is the display
	~ is the delimiter 

Equations in abstracts
* You cannot add special characters to the title :( but we can do it in abstracts~
* there is a module called MathJax (https://www.mathjax.org/) it lets you write in LaTeX and renders it pretty. 
* this works for screen readers
* question: concern, you can turn stuff off, but how much do we want to enable upfront vs. having recipes for IR. this is a bit nichefor IR side that some institutions. 
* it would be good to have an recipe for IR for the starter site. the  iR group has had come conversation about this, however it's unclear the conversation bout it. 
* question: how does abstract work with non-latin text? it might already be built in. 
* the ability to have title field that accommodates this would be nice (example, a title in arabic, or a title with math equations in it). 
* like idea recipe. where would we store it? should we store it? should we put it in our cookbook? does it need tob e drupal, or just an "install this module" 
* we could put this in the islandora documentation recipe page

Title
* Rosie was working on title field and replicating MODS
* lets vote on priorities
* italics and bold
* unlv uses : https://www.drupal.org/project/html_title 
	* does this make a rich field? does not change field type (drupal will now let you do that), but allows you to put in some tags you allow, then it will convince drupal to render it as html instead of escaping it (as it currently does)
	* will it change tab title of webpage? unclear
* Rosie will text out and do a PR

Open Discussion
* ASU - working for new content model for scholarly content. it's mostly ready to go other than styling and migration code. 
	* instead of having complex object, the structure - they have a media reference field opposed to media pointing to node
	* this helps with google analytics -- so anytime someone clicked on the child of an object, google analytics now counts it as visiting the parent, opposed to earlier the child was separate from the parent
	* for thumbnails, using drupal thumbnail system opposed to islandora derivatives. with drupal, there is a module that allows you to do documents. 

* PEI -mapping data object 
* Whitman - lots of clean up of metadata on the back end

Glossary
* GUI, Linked Agent, Islandora Model


### Next meeting
August 26, 2024 
