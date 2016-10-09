# link-replace-after-migration-wordpress

update table_name set field_name = replace(field_name, 'original text','replacement text');



update wp_posts set posts_content = replace( posts_content, 'http://oldurl.com/', 'http://newdomain.com/subfolder/');  
update wp_links set link_url = replace( link_url, 'http://oldurl.com/', 'http://newdomain.com/subfolder/');  
update wp_postmeta set meta_value = replace( meta_value, 'http://oldurl.com/', 'http://newdomain.com/subfolder/');  
update wp_options set option_value = replace( option_value, 'http://oldurl.com/', 'http://newdomain.com/subfolder/');  
update wp_comments set comment_content = replace( comment_content, 'http://oldurl.com/', 'http://newdomain.com/subfolder/');  



 
wp_posts table, in the posts_content field (links inside posts and pages)  
wp_links table, in the link_url field (the old Link Manager)  
wp_postmeta table, in the meta_value field (URLs of Custom Menu items)  
wp_options table, in the option_value field (anything saved by themes and plugins)  
wp_comments table, in the comment_content field (URLs inside comments)  

