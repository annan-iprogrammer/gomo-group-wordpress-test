Wordpress steps setup website
1. Clone the Project from Git
    - git clone https://github.com/annan-iprogrammer/gomo-group-wordpress-test.git
2. Configure wp-config.php 
3. Set Up Database and import the DB Dump
4. Update Site URL from DB 
    - UPDATE wp_options SET option_value = 'your local/stage url' WHERE option_name IN ('siteurl', 'home');
5. Elementor → Tools → Replace URL
