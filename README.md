# **CSS Flexbox Photo Gallery Project**
#### learned it from [freeCodeCamp](https://www.freecodecamp.org/)
###### Flexbox helps you design your webpage so that it looks good on any screen size. In this course, you'll use Flexbox to build a responsive photo gallery webpage.
---
### **Overview**  
The **CSS Flexbox Photo Gallery Project** is a web-based application that displays a collection of photos in a responsive gallery layout. This project leverages HTML for structure and CSS Flexbox for creating a clean, user-friendly, and adaptable grid of images.

---

### **Table of Contents**
1. [Project Structure](#project-structure)  
2. [HTML Details](#html-details)  
3. [CSS Details](#css-details)  
4. [How to Use](#how-to-use)  
5. [Summary of Selectors Used](#summary-of-selectors-used)

---

### **Project Structure**  
The project consists of two main files:  

- **`index.html`**: Contains the structure of the gallery.  
- **`styles.css`**: Defines the layout and visual styles using CSS Flexbox.

**File structure:**  
```
/
├── index.html
├── styles.css
```

---

### **HTML Details**  
The `index.html` file structures the content of the photo gallery.

#### Key Elements:
1. **Header**:
   - Displays the title of the gallery using an `<h1>` tag inside a `<header>` element.
   - Styled for emphasis and visual appeal.

2. **Gallery**:
   - A `<div>` element with the class `gallery` wraps the collection of images.
   - Each image is embedded using the `<img>` tag, sourced from a URL.

**Example:**
```html
<header class="header">
    <h1>css flexbox photo gallery</h1>
</header>
<div class="gallery">
    <img src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/1.jpg" alt="imge1">
</div>
```

---

### **CSS Details**  
The `styles.css` file defines the styles for the gallery layout and design.

#### **General Styles:**
1. **Global Reset**:
   - `box-sizing: border-box` ensures padding and borders are included in element dimensions.
   - `margin: 0` removes default spacing for a consistent layout.

2. **Body**:
   - The `body` is styled with a neutral background color (`#f5f6f7`) and a sans-serif font for readability.
   ```css
   body {
       margin: 0;
       font-family: sans-serif;
       background: #f5f6f7;
   }
   ```

---

#### **Specific Styles:**
1. **Header (`.header`)**:
   - Center-aligned text with uppercase transformation for the title.
   - Uses a dark background with contrasting text and an orange border at the bottom.
   ```css
   .header {
       text-align: center;
       text-transform: uppercase;
       padding: 32px;
       background-color: #0a0a23;
       color: #fff;
       border-bottom: 4px solid #fdb347;
   }
   ```

2. **Gallery Container (`.gallery`)**:
   - Implements Flexbox properties:
     - `display: flex` to enable a flexible layout.
     - `flex-wrap: wrap` ensures images wrap to the next row when necessary.
     - `justify-content: center` centers the gallery content.
     - `gap: 16px` adds spacing between images.
   - Constrained to a `max-width` of 1400px for a clean layout on larger screens.
   ```css
   .gallery {
       display: flex;
       flex-direction: row;
       flex-wrap: wrap;
       justify-content: center;
       align-items: center;
       gap: 16px;
       max-width: 1400px;
       margin: 0 auto;
       padding: 20px 10px;
   }
   ```

3. **Images (`.gallery img`)**:
   - Sized responsively with a `max-width` of 350px and a fixed height of 300px.
   - Styled with `object-fit: cover` to ensure the images maintain their aspect ratio without stretching.
   - Rounded corners with `border-radius: 10px` add a polished look.
   ```css
   .gallery img {
       width: 100%;
       max-width: 350px;
       height: 300px;
       object-fit: cover;
       border-radius: 10px;
   }
   ```

---

### **How to Use**

1. **Clone the Project**:
   ```bash
   git clone https://github.com/shadyashraf174/Photo-Gallery
   cd Photo-Gallery
   ```

2. **Run the Project**:
   Open the `index.html` file in a browser to view the photo gallery.

3. **Customization**:
   - Add or replace image URLs in the `<img>` tags to modify the gallery content.  
   - Adjust the `max-width` or `gap` in `.gallery` for different layouts.  
   - Change colors in the `.header` to match your desired theme.  

---

### **Summary of Selectors Used**

#### **Tag Selectors**:
- `body`: Styles the overall page layout and background.

#### **Class Selectors**:
- `.header`: Styles the gallery title and header section.  
- `.gallery`: Defines the Flexbox layout for images.  
- `.gallery img`: Applies size and appearance styles to the gallery images.

#### **Pseudo-Elements**:
- `.gallery::after`: Adds an empty pseudo-element for layout purposes.
---

![image](https://github.com/user-attachments/assets/e381c452-1c19-4a22-a2ba-026c147624c6)

---
This project showcases the power of CSS Flexbox for building a responsive and visually appealing photo gallery. It is beginner-friendly and can be easily customized for different photo collections.
