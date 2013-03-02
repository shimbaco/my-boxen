# This file manages Puppet module dependencies.
#
# It works a lot like Bundler. We provide some core modules by
# default. This ensures at least the ability to construct a basic
# environment.

def github(name, version, options = nil)
  options ||= {}
  options[:repo] ||= "boxen/puppet-#{name}"
  mod name, version, github_tarball: options[:repo]
end

# Core modules for a basic development environment. You can replace
# some/most of those if you want, but it's not recommended.

# Includes many of our custom types and providers, as well as global
# config. Required.

github 'boxen', '1.0.2'

# Core modules for a basic development environment. You can replace
# some/most of these if you want, but it's not recommended.

github 'gcc', '1.0.0'
github 'git', "1.0.0"
github 'homebrew', '1.0.0'
# github 'imagemagick', '1.1.0'
github 'inifile', '0.9.0', :repo => 'cprice-puppet/puppetlabs-inifile'
# github 'mysql', '1.0.0'
# github 'qt', '1.0.0'
# github 'redis', '1.0.0'
github 'stdlib', '3.0.0', :repo => 'puppetlabs/puppetlabs-stdlib'
# github 'sublime_text_2', '1.0.0'
github 'sudo', '1.0.0'
# github 'xquartz', '1.0.0' # qtのインストールで使用
# github 'wget', '1.0.0'

# Optional/custom modules. There are tons available at
# https://github.com/boxen.
