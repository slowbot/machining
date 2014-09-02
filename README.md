Machining
=========

Machining is a method of front end development preferred by the team at Mister Machine. It involves rolling togeher design and development practices.  

Getting Started
-------

* **Sketching**
We still use Photoshop. Raster based desktop aplications are very good at specific operations that allow for free asscoaition and of art direction. 

* **Type**
We encourage the use of Typecast to experiment with font families, sizing and type scale. [Typecast](http://typecast.com)

* **Grid**
We also suggest moving onto Gridlover for layout rules. Once we extract some key numbers from Typecast we experiment with vertical rhytmns and breakpoints. [Gridlover](http://www.gridlover.net)

Setting up a Project
-------

All of our front end developers are required to install a local development environment. This allows the whole team to benefit from source control and contribute to the production environment. 

### Software
* **Github for Mac**
Feel free to use terminal but we like Github for Mac for it's Drag and Drop UI.

* **Sublime Text 3**
Use the text editor of your choice but we like Sublime Text for its feature set and custom options. 

### Molecule Man
We have put together a static site builder that is our boilerplate for projects. It allows us to take advantage of the modular nature of Sass and build our HTML partials accordingly.

* **Middleman**
Rails static site builder. Since we are using Sass and Compass we liek that it is in the same family. 

* **Sass w/Compass**
We find Sass to be the best supported preprocessor with an engaged community helping to define new features. 

* **Atomic Design with OOCSS**
Whichever flavor you prefer, we like our styles DRY. The default Sass structure that comes with Molecule Man is suggested as a starting point. 

* **Style Tile**
Based on the work done so far we want to extract and present the variables which will become the basis of our Pattern Library. These core elements include:
  * Type
  * Color
  * Grid & Rhythm
  * Global elements

Parts Inventory
-------

### Content Audit 
A simple spreadsheet which allows the least technical member of the team to contricbute to the content definition portion of the project.

### Sitemap & Wireframes
We use Slickplan for sitempas and a combination of Balsamiq and InVision for Wireframing. 
http://slickplan.com
https://balsamiq.com
http://www.invisionapp.com

### Blocking
Object modeling allows us to define the building blocks of our content. Again keeping in mind Atomic and OOCSS principles we want to design our products based on their natural material, the content.

We track and define our inventory in a Google Document shared by Product, Design and Development.

  * News site - single article
  * Realty site - single property
 
Define larger groupings of related content
  * Archive, Search
  * Map global elements
  * Header, Footer

### Scribing
Namespacing our components is important. Domain language will be shared across Product, Design and Development

* Use minimal descriptive naming to organize your style into modules
* Nest required classes within a Component class to avoid collision
* Build more specific names using dashes or &-
* Avoid dashing more than 3 levels deep

Pattern Library
-------
We have expanded a pattern library from being a style guide it being the essential Front End Development branch of every project. It is where the brand language is developed as well as where new components are tested.

### Looming
The process for determining our base units will effect the whole or our design. It is the horizontal and vertical grid across all breakpoints.
* Font size ex. 16px
* Character Measure per line ex. 65
* Vertical Line height based on legibility ex. 1.5
* Base Units in both directions (16 x 1.5 = 24px)
* Columns and Gutters ex. 12/24/36/48px

### Tooling
Taking the brand language we defined in our style tile and parts inventory we developed with the team we can now begin to sculpt the individual display components.

* Start with a low resolution HTML site map within the static environment
* Focus on key wireframes to extract new Partials
* Avoid using grid classes on the Partial level to ensure reuse
* Reserve Component definitions to include only high level site content

### Prototyping
When something has to move or tell a story we isolate the necessary components or create a branch off master.

* Include external js files and add function calls to app.js with commenting
* Create a new partial to sandbox interaction styles


SCSS/CSS Guidelines
-------

### Spacing
* Use soft tabs
* Put line breaks between rulesets
* Place closing braces on a new line
* Give each declaration its own line

### Formatting
* Use // for comments
* Avoid units for 0 values
* Avoid nesting more that 4 levels
* Use hyphens instead of underscore in class and filenames
* Use double quotes

### Pixels vs Ems
* Avoid using px independent of rem function
* Generally use rems for type and reserve ems for layout spacing

### ID's vs classes
* Candidates for ids include header, footer
	
### Naming
* Use meaningful names
* Avoid using html tags in class names
* Avoid applying styles to base html tags

### Order
* Use Alphabetcal order
* Exlends
* Includes
* Property: Value
* Psuedo
* Nested elements
* Media Queries
	
### Structure

```shell
/base
	reset.scss
	variables.scss
	typography.scss
	
/tools
	mixins.scss
	functions.scss
	
/components
	/partials
	example.scss
	
/layout
	header.scss
	footer.scss

/pages
	home.scss
	single.scss
	
/helpers
	shame.scss
	
/vendors
	foundation.scss
```		

HTML Guidelines
-------
	
### General
* Whenever possible avoid superfluous parent elements. 

### Forms
* Wrap inputs inside of labels

### Semantics
* Section if a page level element
  * avoid nesting sections within an article
* Article is a single unit of primary content
* Aside is a supplementary page element
	
Structure
```shell
/partials

/components

/layout

/pages
```		
