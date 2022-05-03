# Informations for the one who tries to fix this bug

This is a fresh laravel installation with following modifications
- config/filesystems.php
  - a ftp configuration was added pointing to some public ftp I looked up for showcasing. Any ftp server will do
- routes/web.php:18
  - a write action to the ftp is called. This causes the ErrorException (Bug) 
