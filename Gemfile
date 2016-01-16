# -*- ruby -*-

source "http://rubygems.org"

gemspec

group :test do
  install_if -> { Gem::Requirement.create('>= 2.0.0').satisfied_by?(Gem::Version.create(RUBY_VERSION)) } do
    gem "net-ldap"
  end

  platforms :mri do
    gem "ruby-ldap"
  end
  platforms :jruby do
    gem "jruby-openssl"
  end
end
