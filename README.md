# bounded_context_canvas_md

<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/grjsmith/bounded_context_canvas_md
">
    <img src="images/bounded_context_canvas_md.png" alt="Bounded context canvas funky synthwave logo" width="800">
  </a>

<h1 align="center">Bounded Context Canvas Markdown</h1>

  <p align="center">
    A simplified implementation of the ddd-crew's [Bounded Context Canvas](https://github.com/ddd-crew/bounded-context-canvas) in markdown
    <br />
    <a href="https://github.com/grjsmith/bounded_context_canvas_md"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/grjsmith/bounded_context_canvas_md/issues">Report Bug</a>
    ·
    <a href="https://github.com/grjsmith/bounded_context_canvas_md/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project
[Tomek Paczkowski](https://www.linkedin.com/in/tomekpaczkowski/) and I were trying to create some well defined bounded contexts out of a set of existing systems. This had been tried before with workshops and asking questions with little success. Tomek and I came up with the idea of using [Notion](https://notion.so/) and the bounded context canvas on a call with the engineers who ran the service to try and extract the details. We created a the DDD group's bounded contect canvas in Notion and began using Markdown to enter the details. We used Cunningham's Law* to get the engineers to actively contribute and eventually take over the exercise and populate the information for themselves. This not only worked beautifully but it took us less than an hour to get a good first draft of each bounded context.

\* "The best way to get the right answer on the Internet is not to ask a question; it's to post the wrong answer." - [Howard G Cunningham](https://en.wikipedia.org/wiki/Ward_Cunningham#:~:text=%22Cunningham's%20Law%22,-For%20the%20mathematical&text=Cunningham%20is%20credited%20with%20the,than%20to%20answer%20a%20question.)
<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

* The ddd-crew's [Bounded Context Canvas](https://github.com/ddd-crew/bounded-context-canvas).
* We used [Notion](https://notion.so/) because that was the document management tool of choice in Pollen. This could be done in VSCode or any text editor with Markdown support. 

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started
### Prerequisites

The only prerequisites required are the courage to look stupid in front of engineers and a willingness to frustrate them a little before they get the hang of it and take over.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage
# 101 Ways Bounded Context Canvas Template

Created: Grant Smith

Created at: February 4, 2022

# <Name> bounded context canvas

# Description

>What benefits does this context provide and how does it provide them

# Ubiquitous language

>Context specific domain terminology

- *Domain term: Definition*
- *Domain term: Definition*
- *Domain term: Definition*

# Inbound data
### Data provided by another context
```yaml
# employee data
   employee_id: 1234
    name: John Smith
     contact: 
       home: 02012345678
       office: 02087654321
     role: Software Engineer
     office_address: 
       street: "145 City Rd"
       town: London
       post_code: EC1V 1AZ
     employed: True
```
### Data provided by another context

```yaml
# skills data
   employee_id: 1234
   skills:
     - Javascript
     - Azure
     - Github Actions
```
## Events consumed
- EmploymentStatusUpdated
- EmployeeSkillsUpdated

# Business rules

1. If skills include 'Azure' raise event AzureDevOps
2. ...

# Outbound Data
```yaml
# Talent Availability Object
employee_id: 1234
   skills:
     - Javascript
     - Azure
     - Github Actions
   Region: SE
   available_for_work: True
   work_type: [ "Front-end Engineering", "DevOps" ]
```
## Events published
- FrontendEngineerAvailable
- DevOpsEngineerAvailable 

# Assumptions

Talent team are specifically interested in Azure DevOps capability

<p align="right">(<a href="#top">back to top</a>)</p>-->

<!-- ROADMAP -->
## Roadmap

Still working on Gotop config
Tempted to figure out the Terminal weather app.

See the [open issues](https://github.com/grjsmith/bounded_context_canvas_md/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- LICENSE -->
## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Grant Smith - [@grjsmith](https://twitter.com/grjsmith) - grant@nextgendevops.com

Project Link: [https://github.com/grjsmith/bounded_context_canvas_md/](https://github.com/grjsmith/bounded_context_canvas_md/)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments
* Thanks to the [ddd-crew](https://github.com/ddd-crew/)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->