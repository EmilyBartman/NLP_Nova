# Final Report: NLP Nova - Make a Hero
By Emily Bartman, Saad Azeem, & Kanin Bender

## Purpose and Audience
The purpose of this application is to empower users to create unique superhero names and backstories based on their envisioned traits, powers, and gender preferences. This tool bridges the gap between imagination and linguistic creativity, offering a platform for entertainment and inspiration. The audience includes hobbyists, creative writers, and individuals seeking personalized storytelling experiences.

## Application Architecture
The final application architecture reflects significant evolution from earlier stages:

**Frontend:**
- Midway Status: Basic HTML templates with limited styling and input functionalities.
- Final Stage: Fully designed and styled web interface with clear navigation and interactive forms.

**Backend:**
- Midway Status: Initial hero name generation implemented using static logic. Limited backend integrations with external services.
- Final Stage: Dynamic name generation and backstory creation leveraging OpenAI GPT-4O. Improved logic for inclusive and meaningful name generation.

**Deployment:**
- Midway Status: Local execution with minimal deployment considerations.
- Final Stage: Google Colab deployment with Ngrok integration for public access.

## Functionalities

**Hero Name Generation:**
- Midway Status: Functional but lacked diversity and inclusivity in name suggestions.
- Final Stage: Improved logic for unique names with gender-based inclusivity, ensuring personalization and avoiding repetition.

**Hero Backstory Generation:**
- Midway Status: Planned but not yet implemented.
- Final Stage: Fully functional backstory creation using OpenAI GPT-4O, generating engaging and coherent superhero narratives.

**Interactive Interface:**
- Midway Status: Limited functionality with placeholder input forms.
- Final Stage: Polished and user-friendly interface with separate sections for name and backstory generation.

## Links
- **Colab Link:** NOT_SHARED_PUBLICLY
_Note: This link is for grading purposes only and should not be shared or used outside this context._
- **GitHub Repository:** https://github.com/EmilyBartman/NLP_Nova/tree/main
_Note: API keys and Ngrok tokens are omitted in the publicly available code._
- **Video Presentation:** [ SAMPLE VIDEO PLACEHOLDER https://youtu.be/zRplfZGIOS4 ]

## Challenges and Resolutions

**Unresolved Challenges (Midway Status):**
- Hero backstory generation was not implemented.
- Deployment was limited to local execution.
- Input processing logic for name generation was basic.

**Resolutions (Final Stage):**
- Hero backstory generation was completed using OpenAI GPT-4O.
- Google Colab was integrated for deployment, allowing public access with proper credentials.
- Name generation logic was enhanced to include dynamic prefix and suffix selection with gender inclusivity.

## Project Reflection Insights

**Alignment with Proposal:**
- The final application meets the proposed objectives of name and backstory generation, demonstrating significant progress from the midway point.

**Stretch Goals:**
- The stretch goal of backstory creation was achieved, marking a milestone beyond initial expectations.

**Limitations:**
- Real-time chatbot functionality (originally part of the stretch goal) was deprioritized to focus on name and backstory generation.

## Issues and Contributions
### Issues:

- **Authentication Requirements:** OpenAI API key and Ngrok authentication token are essential but omitted in the publicly available code for security reasons.
- **Colab-Specific Configuration:** The app is tailored for Google Colab, requiring adaptation for local or production deployments.
- **Loading Delays:** When the generation engages with the model to assist in some app functions like the backstory generation, it can take a few minutes to give results. 

### Contributions (Final Phase)

**Emily Bartman:** Integrated OpenAI GPT-4O into the backend to enable seamless story generation, and refined the backend logic for hero name creation. Developed and styled the interactive web interface, ensuring smooth user interactions and a cohesive user experience. Reviewed code and assisted in final report and presentation creation.

**Saad Azeem:** Laid the foundational logic for hero name generation, which was later enhanced by integrating the GPT-4O model. Contributed to optimizing the algorithm for dynamic and inclusive name generation. Reviewed code and assisted in final report and presentation creation

**Kanin Bender:** Established the groundwork for backstory generation by researching and evaluating different approaches. Helped identify the optimal use of GPT-4O for generating compelling and coherent superhero origin stories. Reviewed code and assisted in final report and presentation creation

## References
- **Superheroes NLP Dataset:** Used as inspiration for hero names and traits. Available on Kaggle by Jonathan Besomi (2020).
- **OpenAI GPT-4O:** Core engine for generating backstories and assisting in debugging and optimization.
- **Ngrok Documentation:** Used for deploying the app via a public URL for user interaction.
