Bozu User Contact Methods

## Show in content
Add this code where you want to show the content
````
<!--
- Detect plugin Bozu User Contact Method
- Check if there is a 'location' author meta
- Show 'location' author meta -->
<?php include_once( ABSPATH . 'wp-admin/includes/plugin.php' ); ?>
<?php if ( get_the_author_meta( 'location' ) && is_plugin_active( 'bozu-user-contact-methods/bozu-user-contact-methods.php' ) ) : ?>
  <em class="author-location icon-location"><?php echo get_the_author_meta( 'city' ); ?></em>
<?php endif ; ?>
````
