Bozu User Contact Methods

## Show in content
Use ''''get_the_author_meta()'''' for rendering the user contact methods
Add this code where you want to show the content for 'location':
````
<!--
- Detect plugin Bozu User Contact Method
- Check if there is a 'location' author meta and plugin Bozu User Contact Method
  is active.
- Render 'location' author meta -->
<?php include_once( ABSPATH . 'wp-admin/includes/plugin.php' ); ?>
<?php if ( get_the_author_meta( 'location' ) && is_plugin_active( 'bozu-user-contact-methods/bozu-user-contact-methods.php' ) ) : ?>
  <em class="author-location icon-location"><?php echo get_the_author_meta( 'location' ); ?></em>
<?php endif ; ?>
````
