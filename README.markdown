Put this in your .bashrc (or whatever bash config file is on your system)

<pre>
function railsapp {
  appname=$1
  shift 1
  rails new $appname T --skip-bundle -m https://github.com/robzolkos/rails-template/raw/master/apptemplate.rb $@
}
</pre>

Then to create a new Rails app :

<pre>
railsapp appname
<pre>
