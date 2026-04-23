# Inner Circle Tavern - Website Management

## Adding Gallery Images

The gallery section on the homepage is hidden by default. Follow these steps to activate it and add your images:

1. **Prepare Images**: 
   Create a folder named `images` in the root directory and place your photos there (e.g., `images/gallery-1.jpg`).

2. **Enable Gallery**:
   Open `index.html` and locate the `<!-- Gallery Section Placeholder -->` block (around line 75).
   - Uncomment the `<section>` and `<div>` block.
   - Remove the `hidden` class from the `<section>` tag.

3. **Add Image Elements**:
   Inside the `<div class="grid grid-cols-2 md:grid-cols-4 gap-4">`, add an `<img>` tag for each photo using the following template:
   ```html
   <img src="images/your-image.jpg" alt="Gallery Image" class="w-full h-48 object-cover rounded-xl border border-white/10">
   ```

4. **Customize Layout**:
   The grid is set to 2 columns on mobile and 4 columns on desktop (`grid-cols-2 md:grid-cols-4`). You can adjust these Tailwind classes if you want more or fewer columns.

## Project Structure
- `index.html`: Homepage
- `menu/index.html`: Restaurant menu
- `reference-only/`: Design system and style guide
