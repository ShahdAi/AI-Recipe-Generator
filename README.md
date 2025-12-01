
# AI Powered Recipe Generator & Calorie Calculator

This project is an AI-powered system that generates personalized meal recipes based on user-defined calorie limits and selected ingredients. It also generates a realistic food image using modern generative AI models. The system combines NLP-based recipe generation with image synthesis and is implemented as an interactive Gradio web application.

## 🚀 Features
- Calorie-based ingredient filtering
- Ingredient suggestions from a nutritional database
- GPT-2 powered recipe generation
- Stable Diffusion image generation
- Fully interactive Gradio interface
- Structured recipe output with title, steps, and ingredients
- Automated prompt construction for consistency and accuracy

---

## 📊 Project Workflow

1. User inputs target calorie amount through the Gradio interface.
2. System retrieves ingredient options and calorie values from a nutritional database.
3. User selects ingredients.
4. GPT-2 generates a structured recipe based on selected items.
5. Stable Diffusion creates a realistic image of the meal.
6. Final output: AI-generated recipe + food image.

---

## 🧠 Model Architecture

### **Recipe Generation (NLP)**
- Model: Fine-tuned GPT-2 (Hugging Face)
- Input: Structured ingredient prompt
- Output: Recipe title, steps, and instructions

### **Image Generation**
- Model: Stable Diffusion (Hugging Face API)
- Input: Recipe + ingredient keywords
- Output: Realistic meal image

### **Non-ML Components**
- Calorie filtering logic  
- Nutritional dictionary  
- Prompt builder  
- Input validation  
- Gradio web UI  

---

## 📚 Dataset
**Food.com Recipes Dataset** (230K+ recipes)  
Includes:
- Recipe titles  
- Ingredients  
- Instructions  
- Nutritional values  

Dataset reference:  
https://www.kaggle.com/datasets/shuyangli94/food-com-recipes-and-user-interactions

---

## 🛠️ Technologies Used
- Python
- GPT-2 (Hugging Face)
- Stable Diffusion
- Gradio
- NumPy / Pandas
- Food.com Dataset
- OpenAI & Diffusion API integration

---

## 📈 Performance Metrics
- **BLEU Score:** 0.059  
- **ROUGE-L:** 0.316  
- **CLIP Score:** 1.0 (strong alignment between text and generated images)

These evaluations indicate strong image-text consistency and reasonable recipe coherence for NLP-based generation.

---

## 🧪 Example Outputs

### Example 1  
User Calories: 800  
Selected Ingredients: rice, avocado, chicken, potato  
**Result:**  
- GPT-2 generated a clear, organized recipe  
- Stable Diffusion generated an image closely matching selected ingredients  

### Example 2  
User Calories: 450  
Various ingredient combinations tested—system responded flexibly and consistently.

---

## ⚠️ Challenges
- Limited calorie accuracy due to static nutritional values  
- Restricted ingredient diversity  
- Occasional vague instructions from GPT-2  
- Image may not always perfectly reflect recipe details  
- No dietary filters (vegan, gluten-free, allergies)  
- No macro breakdown (carbs, protein, fats)

---

## 🔭 Future Improvements
- Integrate live nutritional APIs (USDA, Edamam)  
- Add dietary preference filters  
- Mobile app version  
- Arabic language support  
- Voice interaction  
- Advanced constraint-based recipe generation  

### 🎥 Demo Video
Click below to watch the project demo:

[Watch the video](demo/demo_video.mp4)

---

## 👩‍💻 Project Members
- Shahd Altamimi  
- Layan Alshaheen  
- Shouq Aldossari  
- Reema Alkathiry  
