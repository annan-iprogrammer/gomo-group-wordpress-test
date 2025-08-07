# WordPress Website Setup Steps

Follow these steps to set up the WordPress website locally or on a staging environment.

## 1. Clone the Project Repository

```bash
git clone https://github.com/annan-iprogrammer/gomo-group-wordpress-test.git
```

## 2. Configure `wp-config.php`

Update the following details in the `wp-config.php` file:

- Database name
- Database username
- Database password
- (Optional) Other environment-specific settings

## 3. Set Up the Database

- Create a new database in your local/staging environment.
- Import the provided database dump file into the new database.

## 4. Update Site URL in the Database

Run the following SQL query to update the site URL:

```sql
UPDATE wp_options 
SET option_value = 'http://your-local-or-staging-url.com' 
WHERE option_name IN ('siteurl', 'home');
```

## 5. Update URLs in Elementor

- Navigate to `Elementor → Tools → Replace URL`.
- Replace the old site URL with your local/staging URL.

## 6. Admin login details 

- User Name: inter@medics
- Password: an09ek5TQ@HD5U

---