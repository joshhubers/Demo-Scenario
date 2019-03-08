# The Dino Asset Tracker 9000

The local museum head paleontologist has decided to revamp their research and engagement programs. Their current processes are outdated, mostly circling around something called "paper" and "filing cabinets." He would like to not only update their asset manangement system for keeping stock of inventory (mostly dinosaur bones), but also provide a simple easy-to-use interface for for those who visit the museum and would like to know more about their exhibits. He dreams of having two components to this application.

The first and largest priority is asset and research management. This will compose about 80% of the project. For the initial pilot of this application only the paleontology department will be using this application. (Note that these are just the things "PHB" cares about and may or may not reflect actual implementation or design of the system, that is up to you to decide!).

## Assets

They would like a web portal where their researchers can see details of their collection of bones and artifacts discovered and contributed to the museum. Assets have the following characteristics:
- Identification Number. This is a GUID value that identifies the asset.
- Name. The scientific name for the asset.
- Secondary Name. A more common or recognized name for the asset.
- Era. The predicted era from which this asset is from
- General Notes. General details of what this asset is.
- Current Location. Where this asset is. Whether in an exhibit, storage, a lab, or on loan.
- Credited Founder. The person or researcher who is attributed to finding this asset.

### Dinosaurs

__I'm a paleontologist not a physicist!__ A dinosaur has the following characteristics:
- Identification Number. A GUID value that identifies the asset.
- Scientific Name.
- Common Name.
- Era.
- Description.
- Current Location.
- Notes.
- Bones. The bones this dinosuar is made of.
- Artifacts. A potential collection of "things" that are also related to this dinosuar. (eggs, feathers, trace fossils, etc.)

### Researchers

Paleontologists are people too. The head paleontologist would eventually like the system have a system for the researchers to login, and eventually even visitors of the museum to maybe even see details of their careers.
- Name.
- Occupation.

# Functionality

The head hancho would like the web portal for researchers to manage these assets and dinosuar information. Editing their basic information, adding notes, and getting basic information for them. They envision a system that is easy to search for assets and dinosuars by their identifier, names, era's, and other basic properties.

### Stretch goal functionality

The musuem will be replacing their exhibit displays with basic display screens. This would make it much more convential for swapping out exhibits. They would like the system to have a "kiosk view" of the basic information for guests to read and view about the contents of the exhibit.

# Technical Implementation

> Of course you can use any language and framework, however these are the technologies I have chosen.

Your mission (if you so choose to accept it), is to make this web application.

### Backend

- [Microsoft Dotnet Core](https://docs.microsoft.com/en-us/aspnet/core/?view=aspnetcore-2.2)
- [Json Api Dotnet Core](https://github.com/json-api-dotnet/JsonApiDotNetCore)
- For quick and easy development I would look at using the [Sqlite Entity Framework Provider](https://docs.microsoft.com/en-us/ef/core/get-started/netcore/new-db-sqlite)

### Frontend

- [Ember JS](https://emberjs.com/)

### Testing

Code should be tested and not considered "production ready" until so. Two frameworks for testing:
- [Xunit](https://xunit.github.io/)
- [Ember Mirage](https://www.ember-cli-mirage.com/)

## Stretch Goals
- Dockerized/Containerized application
  - [Docker](https://www.docker.com/)
- Deployed to a cloud/server environment
- Application Authenticiation
  - [Dotnet Core Identity](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/identity?view=aspnetcore-2.2&tabs=visual-studio)
  - [Ember Simple Auth](http://ember-simple-auth.com/)
