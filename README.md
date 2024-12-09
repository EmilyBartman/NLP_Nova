# NLP Nova - December 8, 2024

## Final Report: NLP Nova - Make a Hero

By Emily Bartman, Saad Azeem, & Kanin Bender

---

## Purpose and Audience

The purpose of this application is to empower users to create unique and inclusive superhero names and backstories tailored to their envisioned traits, powers, and gender preferences. By integrating advanced natural language processing (NLP) technology, the app ensures gender inclusivity in hero name generation, celebrating diversity and personalization. This tool bridges the gap between imagination and linguistic creativity, enabling users to craft heroes that resonate with their vision. Designed for entertainment and inspiration, the platform appeals to hobbyists, creative writers, educators, and anyone seeking personalized storytelling experiences. Additionally, its intuitive interface and dynamic customization features make the app accessible and engaging for users of all skill levels.

---

## Application Architecture

The final application architecture demonstrates significant advancements in design, functionality, and deployment, compared to earlier stages of development:

### **Frontend**
Where we were, last submission:
- Implemented basic HTML templates.
- Minimal styling with limited input forms for name and power selection.
- No advanced user feedback mechanisms or interactivity.

Final Code: 
- Developed a fully styled, intuitive web interface using HTML and integrated dynamic interaction through Python scripts in Colab.
- Clear navigation for users to access hero name and backstory generation workflows.
- Interactive forms designed for seamless input, with validation for gender, powers, and preferences.
-	Improved accessibility with tooltips and prompts guiding users through the process. Fully designed and styled web interface with clear navigation and interactive forms.
### **Backend**
Where we were, last submission:
- Static logic for hero name generation without external data or dynamic inputs.
- Backend integrations limited to placeholder scripts for functionality testing.

Final Code: 
- Fully integrated OpenAI GPT-4O API for dynamic generation of superhero names and backstories, providing engaging and coherent results.
- Enhanced name-generation algorithm includes dynamic prefix and suffix logic for gender inclusivity and personalization.
- Created modular functions for handling inputs and generating output, ensuring reusability and maintainability.
- Streamlined data flow from user inputs to GPT-4O interactions, reducing latency during generation.
- Included error-handling routines for missing or invalid inputs, providing user feedback when issues arise.
### **Deployment**
Where we were, last submission:
- Execution was restricted to local machines with minimal considerations for scalability or public access.
- Limited debugging options and no deployment for external users.

Final Code:
- Deployed on Google Colab for ease of access, leveraging Ngrok for public-facing URLs.
- Ngrok Integration: Enabled secure tunneling, allowing the app to function as a web service while hiding sensitive credentials.
- Documentation provided for setting up the Colab environment, including installation of required libraries (e.g., Flask, OpenAI) and securing API keys.
- Deployment includes auto-restart logic for ensuring service continuity in temporary sessions.
- Emphasis on lightweight dependencies, making the deployment process efficient for grading and testing purposes.

The evolution in architecture demonstrates a balance between functionality, scalability, and accessibility, transitioning from a basic prototype to a polished, user-ready application. The focus on user experience, security, and dynamic content generation highlights the comprehensive improvements achieved during the project.

---

## Functionalities

### **Hero Name Generation** - Implemented dynamic hero name generation leveraging OpenAI GPT-4O API:
-	User inputs include hero powers and gender, which are processed to create personalized and meaningful names.
-	The algorithm generates unique names by combining prefixes, suffixes, and thematic patterns influenced by user inputs.
-	Ensures diversity and inclusivity by tailoring name generation logic to align with the specified gender and power set.
-	Built-in mechanisms prevent repetitive or generic name outputs, improving user experience.


### **Hero Backstory Generation** - Fully functional backstory generation uses OpenAI GPT-4O to craft engaging superhero origin stories:
-	Inputs include the hero's name, powers, and gender, ensuring the backstory aligns with the user's vision.
-	Outputs are coherent and well-structured narratives with unique elements such as the hero’s challenges, motivations, and achievements.
-	Includes a modular pipeline to handle multiple queries seamlessly, ensuring smooth interaction with the NLP model.
-	Customizable story archetypes (e.g., heroic, tragic) were conceptualized but not fully implemented in this version.


### **Interactive Interface** - A polished and user-friendly interface designed for ease of use:
-	Separate sections for hero name and backstory generation provide clear navigation for users.
-	Input forms include fields for hero traits such as powers, gender, and name preferences, guiding users through the creation process.
-	Real-time feedback ensures users understand input requirements and receive immediate results.
- Responsive design allows the interface to adapt to different devices when deployed via Colab.
-  Interactive buttons trigger backend logic to fetch and display results, maintaining a seamless connection between the user interface and backend processes.


These functionalities showcase the integration of advanced NLP capabilities with intuitive design, allowing users to effortlessly create heroes with unique names and compelling backstories. The modular approach ensures scalability for future feature enhancements.

---

## Links

- **Colab Link (Working App)**: LINK_NOT_SHARED_PUBLICLY
  - This link is intended for grading purposes only. The app runs locally with free Ngrok integration.
  - The correct Ngrok-generated public link (e.g., `https://xxx-xx-xxx-xxx-xx.ngrok-free.app`) is provided when the Colab notebook is executed. After navigating to the Ngrok link, click the blue button to proceed.

- **GitHub Repository (Public Code)**: [GitHub Repository](https://github.com/EmilyBartman/NLP_Nova/tree/main)  
  - API keys and Ngrok tokens have been omitted for security reasons. Users will need their own credentials to run the app locally or in Colab.

- **Video Presentation (Public Video)**: [YouTube Video](https://youtu.be/-nNPl6T5Uvs)  

---

## Challenges and Resolutions

### **Challenges**

The development of the "NLP Nova - Make a Hero" app involved overcoming several technical and design challenges. Below are the key challenges and their resolutions, enhanced with additional details:

1. **Hero Backstory Generation**:
   - Initially, there was no implementation of backstory generation.
   - The team struggled to determine the optimal approach for creating coherent and engaging narratives that align with user inputs.

2. **Deployment Limitations**:
   - During initial phases, the app was limited to local execution, which restricted accessibility and usability for external users.
   - Securing public access while maintaining the confidentiality of sensitive API keys and tokens posed a significant challenge.

3. **Name Generation Logic**:
   -	Early versions used static and simplistic logic for hero name generation, resulting in repetitive and less inclusive suggestions.
   -	Input processing lacked the ability to tailor names effectively based on gender and power combinations.


4. **Colab-Specific Configuration**:
   - 	Deploying through Google Colab required users to set up dependencies, provide their own credentials, and manage Ngrok configurations, which added complexity for non-technical users.

5. **Loading Delays**:
   -  Some functions, particularly backstory generation, experienced delays due to the time required for model processing, impacting user experience.

### **Resolutions**
1. **Hero Backstory Generation**:
   - 	Fully implemented backstory creation using OpenAI GPT-4O, which generates rich, personalized narratives based on user inputs.
   -	Modularized the backstory generation pipeline to ensure smooth integration with the app's interface and other functionalities.

2. **Deployment Integration**:
   - 	Integrated Google Colab for deployment with Ngrok to create a temporary public-facing URL, enabling external access to the app during evaluation.
   -	Ensured secure handling of API keys and Ngrok tokens by requiring users to input their credentials at runtime.
   -	The app generates a specific public URL (e.g., https://xxx-xx-xxx-xxx-xx.ngrok-free.app) during each session. Users must click a blue button to proceed to the free site, simplifying the interaction process.

3. **Enhanced Name Generation**:
   -	Improved the algorithm to include dynamic prefix and suffix selection, ensuring unique and meaningful name outputs.
   -	Introduced gender-inclusive logic and the ability to consider user-defined powers for personalized hero names, enhancing creativity and diversity.

4. **4.	Colab-Specific Enhancements**:
   - 	Created detailed documentation and user instructions to streamline the Colab setup process.
   -	Reduced dependency conflicts and ensured compatibility with Colab’s runtime environment.

5. **Loading Delays**:
   -	While delays persist due to model processing time, the app includes modularized logic to maintain efficient workflows.
   -	Future optimization strategies, such as implementing caching mechanisms or asynchronous processing, were identified to reduce wait times and improve user satisfaction.

These resolutions reflect the team’s ability to address technical challenges and refine the app to meet the project objectives while maintaining a focus on user experience, security, and accessibility.

---
## Future Improvements
With a strong foundation established and stretch goals partially realized, the "NLP Nova - Make a Hero" app is well-positioned for iterative enhancements, such as permanent hosting, chatbot integration, and expanded customization features, ensuring continued alignment with the project’s creative vision and technological potential.
1. **Permanent Hosting**:
   - Move the app to a permanent hosting solution (e.g., AWS, Heroku) to eliminate dependency on Colab and Ngrok, providing seamless and uninterrupted user access.
2. **Chatbot Integration**:
   - Implement a conversational AI feature to assist users in refining hero traits and backstories interactively, enhancing user engagement and creativity.
3. **Story Themes**:
   - Introduce selectable story archetypes (e.g., heroic, tragic, humorous) during backstory generation, allowing users to customize the tone and style of the narrative.
4. **Villain Creator**:
   - Expand the app to include a villain creation module, enabling users to design antagonists that complement their heroes.
5. **Multilingual Support**:
   - Add support for generating names and backstories in multiple languages, broadening the app’s accessibility and appeal to a global audience.
6. **Interactive Backstory Creation**:
   - Allow users to provide more granular inputs, such as personality traits or specific plot points, to generate highly tailored backstories.
7. **Performance Optimization**:
   - Reduce loading delays for backstory generation by implementing model optimization techniques or caching mechanisms to improve response times.

By addressing these future enhancements, the "NLP Nova - Make a Hero" app can evolve into a more robust, interactive, and globally accessible platform for creating superheroes and their stories.

---
## Contributions

**Emily Bartman**: Played a pivotal role in both the backend and frontend development of the "NLP Nova - Make a Hero" app. She seamlessly integrated OpenAI GPT-4O into the backend, enabling the app to generate rich and engaging superhero backstories. Additionally, she refined the backend logic for hero name creation, incorporating dynamic and gender-inclusive features that enhanced creativity and diversity. On the frontend, Emily designed and styled the interactive web interface, ensuring it was polished, intuitive, and user-friendly. Her contributions extended to creating responsive design elements that facilitated smooth navigation and real-time user feedback. Beyond technical contributions, Emily reviewed and debugged code to ensure the app met project objectives and collaborated on the final report and presentation, ensuring they were professional and cohesive.

**Saad Azeem**: Was instrumental in developing the foundational logic for hero name generation. He designed an algorithm that incorporated dynamic prefix and suffix selection, laying the groundwork for future integration of GPT-4O. Saad enhanced this logic by optimizing it for inclusivity and personalization, ensuring the names were aligned with user inputs such as gender and powers. His focus on quality assurance ensured the codebase was robust, as he conducted comprehensive reviews to identify and resolve performance issues. Saad also contributed to the final report and presentation, ensuring the project’s achievements were clearly and effectively communicated.

**Kanin Bender**: Focused on the research and development aspects of the project, playing a key role in the implementation of superhero backstory generation. He explored various approaches to creating engaging and coherent narratives, ultimately identifying GPT-4O as the ideal tool for this functionality. Kanin established the framework for backstory generation, working collaboratively to ensure seamless integration with the app’s backend. He also actively reviewed code to maintain accuracy and consistency throughout the project. Additionally, Kanin contributed significantly to drafting and refining the final report and presentation, helping to articulate the project’s goals, achievements, and future directions with clarity and professionalism.

---

## References

1. [Superheroes NLP Dataset](https://www.kaggle.com/datasets/jonathanbesomi/superheroes-nlp-dataset?utm_source=chatgpt.com)  
2. [OpenAI GPT-4O](https://platform.openai.com/docs/models/gpt-4?utm_source=chatgpt.com)  
3. [Ngrok Documentation](https://ngrok.com/docs)  
4. [Flask Documentation](https://flask.palletsprojects.com/en/stable/)  
5. [Google Colab Documentation](https://research.google.com/colaboratory/faq.html)  
6. [Python Documentation](https://www.python.org/doc/)  
7. [HTML & CSS Tutorials (W3Schools)](https://www.w3schools.com/html/default.asp)  
8. **ChatGPT and Generative AI Tools**: Used for brainstorming and debugging logic.  
9. **Online Tutorials**: Resources from Coursera and YouTube for backend integration and NLP practices.

