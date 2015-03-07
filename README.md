# PhpStorm-LiveTemplates
Collections of PhpStorm-LiveTemplates

## Installation

First, find your configuration folder.

	Windows: <your home directory>\.WebIde<version>\config
	Linux: ~\.WebIde<version>\config
	MacOS: ~/Library/Preferences/WebIde<version>

On my MacOS, it would be `~/Library/Preferences/WebIde80` so you have to adjust commands to your platform. There is a `templates/` directory. It contains XML files with Live Templates.

Create a git repository in the `templates/` dir and pull the templates
```bash
$ cd ~/Library/Preferences/WebIde80/templates
$ git init
$ git remote add origin git@github.com:laravel-china/PhpStorm-LiveTemplates.git
$ git pull origin master
```
If this wouldn't work, you should just backup your templates, clone the repo and merge them manually.

##Forms

**fo** Form open tag
```php
{!! Form::open() !!}
```

**fc** Form close tag
```php
{!! Form::close() !!}
```

**textfield** Text form field
```php
<!--- $VALUE$ Field --->
<div class="form-group">
    {!! Form::label('$NAME$', '$VALUE$:') !!}
    {!! Form::text('$NAME$', null, ['class' => 'form-control']) !!}
</div>
```

**emailfield** Email form field
```php
<!--- $VALUE$ Field --->
<div class="form-group">
    {!! Form::label('$NAME$', '$VALUE$:') !!}
    {!! Form::email('$NAME$', null, ['class' => 'form-control']) !!}
</div>
```

**passwordfield** Password form field
```php
<!--- $VALUE$ Field --->
<div class="form-group">
    {!! Form::label('$NAME$', '$VALUE$:') !!}
    {!! Form::password('$NAME$', ['class' => 'form-control']) !!}
</div>
```

**textareafield** Text area form field
```php
<!--- $VALUE$ Field --->
<div class="form-group">
    {!! Form::label('$NAME$', '$VALUE$:') !!}
    {!! Form::textarea('$NAME$', null, ['class' => 'form-control']) !!}
</div>
```

**hiddenfield** Hidden form field
```php
{!! Form::hidden('$NAME$', $VALUE$) !!}
```

**submitfield** Submit form field
```php
<!--- $VALUE$ Field --->
<div class="form-group">
    {!! Form::submit('$NAME$', ['class' => 'btn btn-primary']) !!}
</div>
```

**req** Require field (add in the attribute array of any form field type to make field required.
```php
'required' => 'required'
```
