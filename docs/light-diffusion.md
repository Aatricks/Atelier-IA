# LightDiffusion-Next: The Simple Start

Before diving into complex node graphs, let's start with a streamlined experience. **LightDiffusion-Next** is designed to be fast, efficient, and unintimidating.

---

## 🕹️ The Interface at a Glance

LightDiffusion-Next focuses on the "Big Three" of image generation:
1.  **The Prompt:** What you want to see.
2.  **The Negative Prompt:** What you *don't* want to see (e.g., "blurry, low quality").
3.  **The Model (Checkpoint):** The "brain" of the AI (SDXL, SD1.5, etc.).

![Screenshot: LightDiffusion-Next UI Layout](images/ld_ui_layout.png)

---

## 🛠️ Your First Generation

Follow these steps to create your first masterpiece:

### 1. Set the Prompt
Type a descriptive prompt. Use commas to separate concepts.
- **Example:** `A futuristic cyberpunk city, neon lights, rain-slicked streets, cinematic lighting, 8k resolution`

### 2. Choose Your Settings
- **Sampling Steps:** 20-30 is usually perfect. Too few and it's blurry; too many and it takes forever.
- **CFG Scale:** Usually between 5 and 8. This controls how strictly the AI follows your prompt.
- **Resolution:** Start with `512x512` (for SD1.5) or `1024x1024` (for SDXL).

### 3. Click "Generate"
Wait a few seconds. Thanks to optimizations like `Stable-Fast`, you'll see your image appear almost instantly!

---

## 💡 Pro Tips for Beginners
- **Keyword Weighting:** In many UIs, you can use `(keyword:1.2)` to make it more important.
- **Aspect Ratios:** Try `768x512` for landscapes or `512x768` for portraits.
- **Styles:** Don't be afraid to add style keywords like "Studio Ghibli," "Cyberpunk," or "Oil Painting."

!!! tip "Try This!"
    Generate an image of "A cozy cabin in the woods during autumn." Then, try adding "snowing" to the prompt and see how the AI adapts the entire scene!

---

[Next: Advanced Nodes with ComfyUI &rarr;](comfyui.md)
