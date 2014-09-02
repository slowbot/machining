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

All of our front end developers are required to install a local local development environment. This allows the whole team to benefit from source control and contribute to the production environment. 

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

* **Atomic Design. SMACCS, BEM, OOCSS**
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
### Sitemap & Wireframes

### Blocking
Define content building blocks. Again keeping in mind Atomic Design. SMACCS, BEM, and OOCSS principles we want to design our products based on their natural material, the content.
  * News site - single article
  * Reality site - single property
   
Define larger groupings of related content
* Archive, Search
* Map global elements
* Header, Footer

### Scribing (Scribing)
Namespacing our components is important. Domain language will be shared across Product, Design and Development

* Use minimal descriptive naming to organize your style into modules
* Nest required classes within a Component class to avoid collision
* Build more specific names using dashes or &-
* Avoid dashing more than 3 levels deep

Pattern Library
-------

### Base Unit Process (Looming)
* Font size ex. 16px
* Character Measure per line ex. 65
* Vertical Line height based on legibility ex. 1.5
* Base Units in both directions (16 x 1.5 = 24px)
* Columns and Gutters ex. 12/24/36/48px

### Workflow (Tooling)
* Start with a low resolution HTML site map within the static environment
* Focus on key wireframes to extract new Partials
* Avoid using grid classes on the Partial level to ensure reuse
* Reserve Component definitions to include only high level site content

### Interactions (Prototyping)
* Include external js files and add function calls to app.js with commenting
* Create a new partial to sandbox interaction styles

