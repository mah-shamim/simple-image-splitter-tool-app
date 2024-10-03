# simple-image-splitter-tool-app
Image Splitter is a powerful PHP script that automates the process of splitting images into smaller grid-based parts. Ideal for creating image puzzles, mosaic art, and other creative projects, this tool features dynamic output directory creation, input validation, and error handling.

**Topics:** `php`, `mysql`, `blog`, `ajax`, `bootstrap`, `jquery`, `css`, `image gallery`, `file upload`, `image-processing`, `data-augmentation`, `image-splitting`, `image-magick`, `drag-and-drop-upload`


![simple-image-splitter-tool-app](./assets/images/simple-image-splitter-tool-app.png)

### Install Process

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/simple-image-splitter-tool-app.git
   ```

2. **Navigate to the Project Directory:**
   ```bash
   cd image-splitter-tool
   ```

3. **Setup Database:**
    - Create a MySQL database named `image_splitter`.
    - Import the provided SQL file to create the necessary table:
      ```sh
      mysql -u yourusername -p image_splitter < db/database.sql
      ```

4. **Update Database Configuration:**
    - Copy `config.sample.php` to `config.php`:
      ```sh
      cp config.sample.php config.php
      ```
    - Open `config.php` and update the database configuration details.

5. **Install ImageMagick:**
    - Ensure ImageMagick is installed on your server.
    - You can check installation using the following command:

   ```bash
   convert --version
   ```

6. **Set Permissions:**
    - Ensure the `assets/uploads` and `output` directories are writable.

   ```bash
   chmod -R 0777 assets/uploads
   chmod -R 0777 output
   ```

7. **Start the development server:**
   ```sh
   php -S localhost:8000
   ```

8. **Access the application:**
    - Open your web browser and navigate to `http://localhost:8000`.
    - Upload an image using the drag-and-drop interface and configure the splitting options.

### File Structure

Here’s a basic file structure for your simple-image-gallery application:

```
simple-image-splitter-tool-app/
│
├── index.html
├── db/
│   └── database.sql
├── src/
│   ├── fetch-image.php
│   └── upload.php
├── include/
│   ├── config.sample.php
│   └── db.php
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── script.js
│   └── uploads/
│   │   └── (uploaded images will be stored here)
├── README.md
└── .gitignore
```