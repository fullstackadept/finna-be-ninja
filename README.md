# finna-be-ninja

Bash scripts to install development environments on Ubuntu/Debian.
These have been used on multiple systems running Ubuntu 14.10, most should work on 14.04 except some package names are different in setup_rbdev.

## Java 8

setup_java

adds the webupd8team key and repository, auto-accepts the license, then installs Oracle Java 8

## Ruby / Build Environment / Rbenv / More Rubies / JRuby

setup_rbdev

Installs numerous packages (from standard apt repos) that Ruby expects, or gems may need for building. Installs OpenSSL, Git, SQLite3/MySQL clients/headers, along with the distro's Ruby/Dev/Rubygems packages.

Also automatically clones and sets up Rbenv in ~/.bashrc

setup_rbenv

Automatically clones ruby-build, then installs Ruby 2.0, 2.1.2 along with Jruby  1.7.18 and the latest 9.0.0.0-pre1. It automatically installs the Bundler gem for each version, and sets 2.1.2 as the global version.


## Mono / ASP.NET

Adds the Mono Project's repos/keys, then installs a complete Mono development environment along with MonoDevelop and the asp.net-examples package.