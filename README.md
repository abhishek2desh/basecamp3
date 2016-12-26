# basecamp3
php wrapper for Basecamp3 , with oAuth 2.0 authentication and some end points covered, with pagination managed internally.

<code>
$client=new Oauth2('clientId','client secret','redirect URL');
$data=$client->get_oauth2_access_token('$_GET['code']');//if using code to fetch access token
OR
$data=$client->get_oauth2_access_token(refresh_token);

####################################################
$data=$client->get_project_list();   // to get the list of all projects visible to the account.

$client->get_todo_list($todo['url']);//give the usrl to get the data from that page, checout the response structure to fetch the URL, usualy found under DOCK:



</code>
