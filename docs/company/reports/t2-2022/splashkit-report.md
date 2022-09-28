## SplashKit

SplashKit is an open-source Software Development Kit (SDK), created with the purpose of reducing the
overhead required for truly technical coding and allowing students new to coding to create
satisfying programs in a short period of time.

SplashKit enables beginning coders to quickly learn to construct fun and functional programs which
they can be proud to showcase. SplashKit is an open-source Software Development Kit (SDK), created
with the purpose of reducing the overhead required for truly technical coding which enables students
new to coding to create satisfying programs in a short period of time. SplashKit enables novice
coders to quickly learn to construct fun and functional programs which they can be proud to
showcase. It includes a large library of functions which can be utilized by the user to experiment
and apply for their own application or game.

This product is currently used by the students at Deakin University and aims to become a global
educational toolkit. Currently the language used for development is C++ and the direction of the
product is to improve and expand the capabilities to increase SplashKit accessibility.

**Product Lead:** Anthony George

### Operations

#### Overview, Goals, and Objectives

The Operations team are responsible for delivering developments at a system level. This includes
foundational project, installation processes ('skm'), bug fixes and solutions to ongoing system
level problems.

This team has a goal of taking last trimesters existing research and extending on that to succeed in
delivering an installation process that is effectively 'one-click' and compatible across all
operating systems.

The team also has the objective to research and document the possibility (or lack thereof) of a
browser based IDE implementation, and should a viable approach exist, design and document an
approach to take to make this feasible.

#### Aims for Trimester

The aim for this trimester is to

- Design a bespoke SplashKit installer
- Develop this as an out-of-the-box SplashKit installer
- Research a browser-based implementation

#### Deliverables

Short-term

- A flow-chart of the intended process
- A UML diagram of the resources required for development
- The foundations of the installer
- Research papers on the possibility of browser based solutions

Long-term

- A 'one-click' SplashKit installer

#### Progress

The Operations team has made great progress so far this trimester, such as:

- Completing the single-command SplashKit installer, meaning we now have single-command installers
  for macOS, Linux, and Windows
- Great progress on GUI installer for Windows using QT framework
- Documenting the new SplashKit install process such that we can update the splashkit.io website
  when the changes are complete
- Researching and documenting the possibility of a browser-based IDE solution with SplashKit
  preinstalled, ala Harvard's CS50 course
  - A viable approach appears to exist but requires further research

The Operations team is working on the following:

- Completing documentation and review of single line installer for Windows
- Finalising new install process instructions for all operating systems
- Squashing a visual bug with the GUI installer for Windows before entering review and documentation
  phase
- Writing research paper on possibility of browser-based IDE solution with SplashKit preinstalled
  - Attempting to get a local prototype running to ensure viability before committing to the
    project, as servers are required

By the end of the trimester the Operations team hopes to:

- Complete the single-command SplashKit installer for all operating systems
- Complete the GUI installer for Windows
- Begin implementing GUI installer for macOS and Linux with QT framework
- Complete the documentation and review of the new install process instructions for all operating
  systems
- Complete the research paper on the possibility of a browser-based IDE solution with SplashKit
  preinstalled
- Progress on a local prototype as proof of concept for the browser-based IDE

#### Final Status

- Single-command installer for macOS, Linux, and Windows completed (awaiting pull request approval to
  merge into master https://github.com/splashkit/skm/pull/46)
- Windows and Linux downloadable GUI installer completed, awaiting creation of new splashkit repo (currently available at https://github.com/Issey9119/SplashKit-Installation-Windows)
  - macOS downloadable GUI installer not yet started due to lack of macOS device to test on (and inability to run in VM), but should be similar to Linux implementation
- SplashKit.io website updated to reflect new install process for single command installers on all operating systems (awaiting pull request approval to merge into master https://github.com/splashkit/splashkit.io/pull/39)
  - Website has also been updated to add a link to download the Windows GUI installer
    - Currently links to an external repo until the new splashkit repo is created
    - Will need to update website again once macOS and Linux GUI installers are completed
- SplashKit browser IDE research completed, and working prototype implemented with Gitpod (available at https://github.com/thoth-tech/splashkit-gitpod-environment)
  - TODO: futher automate the installation of SplashKit in the Gitpod container (specifically automating "skm linux install" following skm install)
  - TODO: Implement NoVNC to emulate GUI for SplashKit programs

#### Project Members (4)

_Delivery Lead:_ Ryan Lawrence

_Developers:_ Ismail Hassan, Auden Vitasa, Kevin Nguyen

### Extensions

#### Overview, Goals, and Objectives

This trimester, the Extensions team will continue to develop the SplashKit translator Ruby
application and enhance it to translate the original C++ library into Python versions > 3.8. The
SplashKit Extensions project’s aim is to provide the SplashKit library interface in additional
languages.

This team has a goal of taking last trimesters existing research and foundation, and extending on
that to succeed in fixing the incompatibilities it encountered.

The team also has the objective to translate other languages if possible, and reserach and develop
an alternative means to the use of MSYS during installation.

#### Aims for Trimester

The aim for this trimester is to

- Understand how the language translators works
- Investigate changes in Python between 3.8x versions and earlier to identify which of these changes
  have caused current incompatibilities
- Get SplashKit successfully working on the latest Python version (3.10.x)
- Fix Python incompatibilities
- Complete Python and Rust language extensions
- Translate to other languages if possible
- Test Python translator

#### Deliverables

Short-term

- Research and document exact versioning errors
- Research and document alternative approaches
- Design and document an alternative approach
- Implement changes to SplashKit-core to rectify incompatibilities

Long-term

- Fix the Python incompatibility on MYSY
- Complete this approach for other languages, preferably Go and Dart

#### Progress

Progress made:

- Finalising the deliverables of Splashkit-Translator from T1 documentation
- Successfully installed and tested Splashkit-Translator with Python and Rust on Splashkit-Core (documented)
- Investigate running Splashkit translator on Windows
- Reviewed Rust library on Splashkit-Core

On-going progress:

- Researching and investigating furthur into Python incompatilibity with MSYS2: "can't locate .dll file"
- Researching the process of the translator, calling from the C native database/library, etc
- Attempting to get Test1 executed wtih Golang from the C native language
- Creating documentation for the processes

Goals for the end of this capstone:

- Fix with incompatibility issue, re-locating the file, creating an environment for the file or via another approach
- Extending the translator language by replicating of Rust library with Go and Dart
- Complete a complete documentation and mannual for the entire process for the next generation

#### Final Status

-

#### Project Members (4)

_Delivery Lead:_ Bella Chhour

_Software Developers:_ Nick Agiazis

### Applications - Arcade Machine

#### Overview, Goals, and Objectives

This trimester, the arcade machine team has a solid foundation to build on, given the creation of a
Windows application capable of cloning the games repository, and executing the games on a playable
interface. The work of last trimester allows the team of this trimester to take closer steps to
creating a physical arcade machine. The machine will perform similarly to a Multi-Game Arcade
Machine, allowing users to select a game from a local library of games. Objectives include:

o Software which:

- Is cross platform compatible
- Allows for game compilation on the host machine
- Is authored to be consistent with a chosen programming convention/style guide
- Implements an architecture that ensures long term maintainability is possible for future
  contributors

o The development of:

- A programming convention / style guide document
- Other General Project Documentation

o Research of:

- Appropriate tooling that can be used to assist with these objectives
- Unit tests and determining if they have any value for the project

Additional features which may be considered later in the lifecycle of the project include the
development and deployment of a website which:

o Supports the uploading of games o Stores and displays:

- User Reviews
- High Scores and Achievements

#### Aims for Trimester

The aim of this trimester is to enhance the existing application to accommodate cross-platform
compatibility. This will include developing methods to facilitate the compilation of games on the
host machine. Access to the game library will be offered through the platform where the user can
configure settings and select and play their desired game. If time permits, a physical Arcade
Machine will be designed and manufactured however the software platform is the primary focus for the
trimester.

#### Deliverables

Short-term

- Decoupling functional behaviour and modularising existing software
- Adding support for all three major operating systems
- Adding support for locally compiled games on the host machine
- Completion of an options menu
- Discussing and agreeing upon a programming convention and style
- Addressing style inconsistencies throughout the project’s source code
- Producing documentation around the project

Long-term

- Physical Arcade Machine built using RaspberryPi

#### Progress

The team have made excellent progress, covering:

- Finalising the automation of the game reviewal process
- Documented a coding standard for developers to follow
- Refactoring codebase to use specified standard
- Refactoring the includes to each respective file that requires them
- Research and documentation on cross platform compatibility
- Refactoring the options menu

The team have also developed:

- Database class for creating databases
- Table class for creating tables
- Methods of standard database queries
- Rating class to handle game rating

Moving forward, the teams goals have shifted to:

- Implementing server based compilation of games
- Implementing realtime loading
- Implementing optional display methods
- Liaising with hardware construction teams
- Developing a design for the hardware

#### Final Status

-

#### Project Members (7)

_Delivery Lead:_ Anthony George

_Software Developers:_ Riley Dellios, Huy Nguyen, Richard Douglas-Denton, Lachlan Foy, Mohamed
Zirufaan, Zac Brydon

### Applications - Build An Exceptional Game

#### Overview, Goals, and Objectives

This trimester, this team will collaborate as a unit to create a single game of exceptional class
and quality.

The goal is to make a game so good it is worthy of commercial release game. The intension here is to
showcase to the world, the power of the SplashKit SDK, and encourage developers to develop games
using the engine. This trimester's student developers will aim to utilise as many methods that
SplashKit has to offer in order to ‘advertise’ SplashKit’s ability as a game engine.

The long-term objectives will showcase how by using SplashKit, game development quality can be
achieved such that the product created is of a high enough professional standard, the game can be
made available commercially. Synchronously, the game will be showcased on the arcade machine in
development.

#### Aims for Trimester

The aim for this trimester is to

- Compartmentalise the tasks to focus teams on specific areas of games development (Design,
  Mechanics, Animations, Collisions, AI, etc)
- Construct UML and foundational designs and specifications
- Generate pixel style artwork acording to references found on Trello and acquire sound assets suitable to specifications
- Game Music is made to fit the style of the game
- Develop the foundations of the game
- Create game functionality, intro animations, menu, options, credits, etc

#### Deliverables

Short-term

- A decided genre of game (1 or 2 player puzzle platform game)
- UML Class diagrams and other designs
- Team creations and task allocations
- Acquisition and creation of assets
- Class creation
- Level Editor created to export level text files.
- Documentation

Long-term

- Commercially releasable game, developed using the Splashkit SDK
- this game will be easily extendable by future teams.
- The current collisions used will be updated to use the new Splashkit rectangle rectangle collision function once available to use.

#### Progress

The team have made excellent progress, covering:

- Design Document including lore of the game 'Below the Surface', design decisions and reference images
- Creating pixel styled visual assets using piskel to create spritesheets of a standard 64x64 size for use in game and level editor
- Music Created appropriate to the style of the game, and more is being made.

The team have also developed:

- A Level Editor that exports level information in a txt file to create new levels
(The Level Editor can use many layers however, 3 is recomended. player, door and enemies must be placed on layer 1)

Moving forward, the teams goals have shifted to:

- Refining the pick up and place function for moving pipes
- Refining the Menu/splash screen and Credits/GameOver screen.
- Refining current levels made to include intuative pipe puzzles
- Creating the HUD displaying the players lives
- Modifying different enemy behaviours to include a jumping enemy (blob monster) and one that doesn't move until it sees the player/s (snake).
- Creating a bonus level where the toxic waste rises over time and player/s may collect bonus lives
- Creating an epic boss battle for level 5
- Game will be uploaded to Arcade Games Reposoitory for use on the Arcade Machine once the above is completed.

#### Final Status

-

#### Project Members (7)

_Delivery Lead:_ Morgaine Barter

_Software Developers:_ Daniel Agbay, Lachlan Morgan, Roy Chen, Robert Osborne, Lily Lan, Jiahao
Zheng

### Modules Enhancements

#### Overview, Goals, and Objectives

The Splashkit modules team has an exciting semester ahead of them, with each module in a position to
have deliverable components completed.

The machine learning module had a working reinforcement learning agent that can play turn based
games. Refactoring and code review was performed on the physics module, but external dependencies on
the Box2D library has left the module requiring a major refactor. This refactor would mean that
Splashkit would contain a native physics engine. The data analytics module has a structure for a
dataframe, pending it passing code review and testing.

Objectives for the modules project include:

- Building multiple machine learning agents utilising different algorithms to be used by developers
  for different features
- Create a 2D physics engine within SplashKit, allowing physics to be easily added to objects within
  a project
- Implement a dataframe structure that loads structured data and create an API that allows a data
  scientist to pre-process, transform and visualise the data.

With the addition of these modules, there is potential for Splashkit to be utilised in a greater
capacity within more disciplines. Building the data analytics module allows for more focused classes
to be designed for data science students, rather than only using Splashkit for building games. Both
the physics and machine learning modules will advance the quality and capability of games and
animations built while using Splashkit.

#### Aims for Trimester

The primary aim for this trimester is to have the reinforcement learning agent ready to use by
developers and to complete the first stage of deliverables for the physics and data analytics
modules. These initial deliverables are to complete the basic dataframe for data analytics and to
replace the existing Box2D library uses with native methods.

Secondary aims for the semester are to create a neural network agent, develop plots and
visualisations from the data in the dataframes and to begin creating methods for gravity, sinking
and projectile motion.

#### Deliverables - Data Analytics

Short-term

- Finish code review
- Load data row by row and column by column
- Working Dataframe with descriptive and transformative methods
- Build a way to display plots and subplots

Long-term

- Fully functioning dataframe
- Data type objects
- Full preprocessing method suite
- Multiple data visualisation methods created
- Integration with machine learning

#### Deliverables - Machine Learning

Short-term

- Create games to test reinforcement learning agent against different game styles
- Begin building neural network agent

Long-term

- Continue adding machine learning models as agents
- Create easy to call methods for developers to utilise these agents

#### Deliverables - Physics

Short-term

- Finish code review
- Refactor code to remove dependency on Box2D
- Create methods for sprite collisions, object collisions and gravity

Long-term

- Create a fully functioning 2d physics engine within Splashkit
- Expand the methods to include physics such as sinking, inertia and others

#### Progress

The modules team has made great progress so far this trimester, such as:

- Data Analytics:
  - Code review that began in trimester 1 of 2022 has been completed. As part of this review,
    recommendations were made on removing string matching and regex code and overhauling the
    dataframe constructor.
  - Redesigning of the dataframe constructor was completed, with potential options for data
    structures discussed in the team. The most efficient choice was to utilise vectors with the
    variant data type.
  - Methods for inserting data into the dataframe column by column and row by row were created and
    tested.
  - Creation of missing documentation and review of current documentation was conducted.
  - Plans for the short term direction of the Data Analytics module were created.
- Machine Learning
  - Upgrades on the matrix_2d library were designed, implemented and tested
  - All current documentation was reviewed and updated where necessary.
  - Plans for the short term direction of the Machine Learning module were created.
- Physics
  - Full review of the existing code for the Physics module has began.
  - Creation of missing documentation and review of current documentation was conducted.

The modules team is working on the following:

- Data Analytics
  - Designing a way for column data types to be manually converted without inserting a new column
    and deleting the old.
  - Creating a custom NULL data type to use in the dataframe. This will work with the current
    exclusive data type column structure.
  - Designing the functionality for dataframes to be populated via comma separated value (CSV) or
    text files. Null and column data types must be completed first.
- Machine Learning
  - Designing a scalable way to calculate the gradient during back-propogation for neural networks.
  - Reviewing the proposed upgrade for the matrix_2d library
- Physics
  - Finalising the review and report on the current Physics implementation (both the existing
    collisions API and the forked Physics API).
  - Designing and implementing methods for rectangle to rectangle collisions. This can be utilised
    by the Build an Exceptional Game team as custom hit-boxes for sprites.

By the end of the trimester the Modules team hopes to:

- Data Analytics
  - Have the functionality to create, display and modify data in the dataframe.
  - Have the functionality to read and write dataframes to and from CSV/text files
  - Design and begin implementing the Data Visualisations API.
- Machine Learning
  - Be able to predict non-linear patterns using a fully connected neural network
  - Be able to use neural networks to create Artificial Intelligence for games
- Physics
  - Have the required methods in the Collisions API created for use in the Build an Exceptional Game
    team
  - Creation of a Gravity API that contains functionality for freefall, terminal velocity and
    sinking.

#### Final Status

-

#### Project Members (8)

_Delivery Lead:_ Timothy Moore

_Software Developers:_ Alex Hocking, Devesh Juggiah, Gaganjeet Singh, Harry Dentry, Jingyu Zhang,
Munatsi Matipano, Kai Tao

---
