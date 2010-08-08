# Gedit Snippets

## PHP

### File Stubs

I've created snippets for generating stubs for Kohana Models, Controllers, and View classes.
You might need to alter them a tiny bit because I've included some things that are specific to the way I work and have structured my projects. But the general idea is that the snippet will parse the path of your file, and name the class appropriately.

The tab triggers are **km** (model), **kv** (view), and **kc** (controller). Creating a file in application/classes/model/user/token.php, then triggering the km snippet will generate the following code for you to begin with.

<pre><code><?php defined('SYSPATH') or die('No direct script access.');

class Model_User_Token extends ORM
{
	public function rules()
	{
		return array
		(
			
		);
	}
}</code></pre>

The ORM text will be highlighted for quick editing, and the cursor will begin inside the rules array.
