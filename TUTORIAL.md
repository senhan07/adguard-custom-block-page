1. **Install Apache2:**
   - For Debian/Ubuntu:
     ```bash
     sudo apt update
     sudo apt install apache2
     ```

   - For CentOS/RHEL:
     ```bash
     sudo yum install httpd
     sudo systemctl start httpd
     sudo systemctl enable httpd
     ```

2. **Navigate to Apache's root directory:**
   - For Debian/Ubuntu:
     ```bash
     cd /var/www/html
     ```

   - For CentOS/RHEL:
     ```bash
     cd /var/www/html
     ```

3. **Clone the GitHub repository:**
   ```bash
   sudo apt install git  # For Debian/Ubuntu
   sudo yum install git  # For CentOS/RHEL

   git clone https://github.com/Gamerou/adguard-custom-block-page
   ```

4. **Copy HTML files to the web server directory:**
   ```bash
   cp -r adguard-custom-block-page/* /var/www/html/
   ```

5. **Adjust permissions if necessary:**
   ```bash
   sudo chown -R www-data:www-data /var/www/html
   ```

6. **Restart Apache to apply changes:**
   - For Debian/Ubuntu:
     ```bash
     sudo systemctl restart apache2
     ```

   - For CentOS/RHEL:
     ```bash
     sudo systemctl restart httpd
     ```

Now, you should be able to access the content of the GitHub repository by visiting your server's IP address or domain in a web browser. If you encounter any issues, let me know!