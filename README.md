# Multi-Agent Customer Support Automation using CrewAI
This project leverages the crewAI AI agents to create a sophisticated support system. These agents provide top-notch support and quality assurance for customer inquiries.

## Installation
To get started, you need to install the required libraries using pip. This includes `crewai`, `crewai_tools`, `langchain_community`, and `langchain_groq`.

## Setup
1. **Import Necessary Libraries:**
   - Begin by importing the required libraries such as crewai, os, and langchain_groq.
2. **Set Up Environment Variables:**
   - Set your GROQ API key using the userdata.get method from google.colab.

## Usage
1. **Define Support Agents:** Create two agents:

 - **A Senior Support Representative** who provides the primary support.
 - **A Support Quality Assurance Specialist** who ensures the quality and completeness of the support provided.
   
2. **Set Up Tools and Tasks:**

- **Tools:** Utilize the ScrapeWebsiteTool from crewai_tools to scrape relevant documentation.
- **Tasks:** Define two tasks:
  - inquiry_resolution: Task for the support agent to resolve the customer's inquiry.
  - quality_assurance_review: Task for the quality assurance agent to review and ensure the response's quality.

3. **Execute the Crew:**

- Define the inputs including the customer, person, and inquiry details.
- Use the crew.kickoff method to start the process and get the final result.

## Example
Here's a simple example to demonstrate the usage:

1. **Define Inputs:** Create a dictionary with customer details and the inquiry.
2. **Kick Off the Crew:** Execute the crew with the provided inputs.
3. **Display the Result:** Use Markdown to display the result in a readable format.
   
## Contributing
I welcome contributions to improve the project. Please fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License.
