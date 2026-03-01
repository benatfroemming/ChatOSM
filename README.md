<img width="1408" height="768" alt="image" src="https://github.com/user-attachments/assets/3bf4315f-78c7-4598-80af-d6be5291025d" />

# ChatOSM

**Explore OpenStreetMap with natural language.**

OpenStreetMap (OSM) is a global, community-driven project that creates and distributes free geographic data for the world. One of the primary ways to access OSM data is through the Overpass API, a read-only interface that allows users to extract specific map features using a specialized query language. While tools like Overpass Turbo make it possible to test queries online, working with OSM data typically requires familiarity with Overpass QL and spatial data concepts. For many users, this creates a significant barrier to entry. ChatOSM removes that barrier by providing a chat-based interface where users can prompt what they want in natural language, such as:

*“Show all mountain peaks in Boulder, CO.”*

*“Find hospitals within 2 km of downtown Minneapolis.”*

*“Map all restaurants that serve pizza in Barcelona.”*

Behind the scenes, ChatOSM translates natural language prompts into structured OpenStreetMap queries and renders the results as interactive maps. This is accomplished through tool calling within an agent-based architecture. The model used in this project is Hermes, an 8B-parameter large language model available on Hugging Face. Hermes is fine-tuned from Llama 3.1 specifically to specialize in structured tool use. Tool calling enables large language models to interact with external systems, APIs, and databases, allowing them to perform actions or retrieve real-time data beyond their training corpus. Instead of generating only conversational text, the model can return a structured JSON object that specifies which tool to call and what arguments to pass.
