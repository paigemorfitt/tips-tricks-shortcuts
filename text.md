Attendees: 

* Chris Day
* Rosie Le Faive
* Paige Morfitt (Notes)
* Amber Arroyo
* Mike Bolam
* Dani Kroon
* Elisabeth Ball
* Joe Corall
* Pascal Brammeier
* Staci Ross



* Have people seen the announcement on the Islandora Lisserv? Yes. 

* Announcements: 
	* we are postponing our demo part 2 for our next meeting


* Open Discussion:
	* Islandora [metadata wish] list(https://docs.google.com/document/d/1nzg6a89LSBunlF0OJLpiRg0tAl1LLI7vP4aYmoJeWpo/edit#heading=h.s9f5ysbwj05o).  Any thoughts
		* Is anyone working on hierarchies with names (example, names are being added in different ways creating individual linked agants, is there a way to link those all together?) 
			* Synnonym module may be of help
			* This may be something the demo would address as well. 
	* Is anyone in the new Islandora working on roles? 
		* Dani (PALS Office) is. Their developers are working on it - they currently have 4 roles. They may have a student worker role in the future. 
	*  Regarding Names and Linked Agents: how are people working with the differing name vocabulary types (corporate, personal, etc) and different models of Islandora (family names, conferences, etc). In all the default versions of Islandora, there is an assumption regarding retaining type vocabularies of names. DGI is hard coaded into CSV template that creates a specific field for name types. Is the logic around that regarding how the name is structured? Does anyone have concerns regarding putting all Linked Agent names into one taxonomy? 
	* Chris (SAIC), always separted out personal names/corporate because they were mapping to MARC, exporting records into worldcat. 
	* Rosie (PEI)doesn't make use of the different vocabularies. Person has birth-death date field, but that information is in the string of the taxonomy. May be personal preference. 
	* Paige (Whitman) keeps separate 
	* Dani (PALS Office) keeps separate - helps with Facets and helps cleaning things up. Also like keepign 100/600/7-- fields separate
	* Mike (Pitt) they are working in large numbers of objects and just had creator fields in spreadsheet. Further complicating, nothing in URI seems to differenciate person/corporate name. Having different buckets/faceting does have it's benifit
	* To add to the complexity of sorting Linked Agents out are local names/names not in LCSH (example, Tribal Names, local names, local companies, etc). 
	* Workbench requires you to add the type ahead of the Linked Agent name (person:creator:NAME)
	* In the form, you cannot create terms on the fly, you have to assign it a type, and a role. Rosie (PEI) defaulted the forms to person, however the forms in Islandora do not. This is complex and goes to the Roles discussion.
	* Conference names: not a lot is heard about people having a specific field for Conference Names. Whitman had a Conference name field, but now just uses Genre to distinguish whether or not something was conference material. 
	* Using views to export Linked Data to get metadata. Next week using Workbench to use export CSV to show  the terms and ids. 

* If there is anything anyone wants to talk about during the meeting, let us know in Slack. We will have a meeting in 2 weeks! 

