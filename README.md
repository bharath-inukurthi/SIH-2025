# Team ID - 61409
## SIH-2025 – Smart India Hackathon 🚀


This repository is created for the purpose of serving as a **single entry point** to my **Smart India Hackathon 2025 (SIH-2025) project**.  

For this project, I have developed **four different codebases** to make the system more **scalable, modular, and maintainable**.  
Instead of keeping everything in one place, each core functionality is built and maintained in a separate repository.  

👉 For convenience, I’ve included all the codebase links here so you can access everything from a single location.  
You can go through them and check out whichever part excites you more — whether it’s **mobile development, backend delivery, admin workflows, or conversational AI**.  

---


# 📊 Feature Status – SIH 2025 Project 

 **Problem Statement (PS) Requirements Implemented** 

| **Feature / Requirement** | **Status** | **Notes / Implementation** |
|----------------------------|------------|---------------------------|
| Multilingual chatbot (Hindi, English, local language) | ☑️ Implemented | Supports English, Hindi, 1 local language |
| Context management across multiple turns | ☑️ Implemented | Session history, session re-initialisation, follow-ups, conversation summaries |
| Fast retrieval and smooth UX for circulars/forms | ☑️ Implemented | Index-based scrollbar, background loading, optimized rendering for 300+ circulars |
| Retrieval-Augmented Generation (RAG) for official emails | ☑️ Implemented | WebSocket chatbot fetching relevant info with citations & attachments |
| Scalable storage and authentication | ☑️ Implemented | Cloudflare R2 for circulars, Supabase Auth for login |
| Daily query/response logs | ☑️ Implemented | Logs stored on VPS |

  **Additional Features Added by Me (Not in PS)** 
 | **Feature / Requirement** | **Status** | **Notes / Implementation** |
|----------------------------|------------|---------------------------|
| Faculty Availability Checker | ☑️ Implemented | Checks if faculty is free in cabin based on timetable data |
| Refactored UI twice (MVP → prod-level) | ☑️ Implemented | Improved user experience |
| Lottie splash animation | ☑️ Implemented | Animated splash screen |
| Caching with Supabase + Redis | ☑️ Implemented | Persistent sessions + active conversation cache |

 **PS Requirements Not Completed Yet** 
| **Feature / Requirement** | **Status** | **Notes / Implementation** |
|----------------------------|------------|---------------------------|
| Human fallback when chatbot cannot answer | ⬜ Not yet | Pending implementation from PS |
| Full multilingual support (≥5 languages) | ⬜ Not yet | Pending implementation from PS |
| Intent recognition | ⬜ Not yet | Pending implementation from PS |
| Embed chatbot on website/messaging platforms | ⬜ Not yet | Pending implementation from PS |
| Advanced privacy/anonymization | ⬜ Not yet | Pending implementation from PS |

---


## 📂 Codebases at a Glance

1. **[React Native App – Transfer Interface](https://github.com/bharath-inukurthi/KARE-BOT-SIH)**  
   The mobile application where users interact with the system.  
   - Faculty Availability Checker  
   - Chatbot Interface  
   - Institution Forms & Circulars Delivery  
   - Accept Class Delivery  
---

2. **[Resource API](https://github.com/bharath-inukurthi/KARE-BOT-Resource-API-SIH)**  
   Acts as the **delivery endpoint** for user requests.  
   - Provides forms, circulars, and download links.  
   - Delivers faculty availability results.  
   - Handles all **resource-related requests** from the mobile app.  

---

3. **[Admin API](https://github.com/bharath-inukurthi/KARE-BOT-Admin-API-SIH)**  
   The **backend processing unit** for institutional data.  
   - Uploads & processes circulars, forms, and timetables.  
   - Extracted timetables are inserted into **Supabase** → can be queried by faculty & time.  
   - Circulars & forms are stored in **Cloudflare R2 buckets** for scalable access.  
   - Manages indexing & organization of institutional resources.  

---

4. **[Chatbot API](https://github.com/bharath-inukurthi/KARE-BOT-Chatbot-API-SIH)**  
   A **dedicated chatbot module**.  
   - Stores user session history for continuity.  
   - Users can revisit past chats and continue in the same context.  
   - Implements **caching with threading** for efficiency.  
   - Powers the chatbot interface in the mobile app.  

---

## 🔗 How to Explore

- Start with the **React Native App** if you’re curious about the **user experience**.  
- Explore the **Resource API** to see how requests are delivered.  
- Dive into the **Admin API** to understand **data processing & storage pipelines**.  
- Check out the **Chatbot API** if you’re interested in **conversational AI & caching techniques**.  

---

## 📌 Note

This repository (**SIH-2025**) itself does **not contain source code**.  
It is created to act as a **central hub** with direct links to all the separate codebases that together form the complete project.  
