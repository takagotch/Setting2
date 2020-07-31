### Setting2
---


```sh
rails new apptky -d postgresql--skip-test-unit
ls apptky
cp -rt apptky /vagrant
rm -rf ~/apptky

vi Gemfile
bundle install
bundle list

time bin/rake about
bin/spring binstub rspec
bin/sprint status
bin/sprint stop

```


```
vi /config/database.yml
rails db:create
rails db:create RAILS_ENV=test
rails s
vi README.rdoc

vi config/application.rb
vi ~/.ssh/hosts
# 127.0.0.1 example.com appkty.example.com
vi spec/spec_helper.rb
```

```sh
vi config/routes.rb
vi config/routes.rb
rails g controller staff/top
rails g controller admin/top
rails g controller customer/top
vi app/controller/staff/top.controller.rb
vi app/controller/admin/top_controller.rb
vi app/controller/customer/top_controller.rb
vi app/views/top/index.html.erb
vi app/views/admin/top/index.html.erb
vi app/views/customer/top/index.html.erb
curl https://localhost:3000/staff
curl https://localhost:3000/admin
curl https://localhost:3000/customer

vi app/views/layouts/application.html.erb
vi app/views/layouts/application.html.erb
vi app/views/shared/_header.html.erb
vi app/views/shared/_footer.html.erb
vi app/helpers/application_helper.rb
vi app/views/layouts/application.html.erb
vi app/assets/stylesheets/application.css
vi app/assets/stylesheets/staff.css
vi app/asets/stylesheets/staff/layout.css.scss
vi app/views/layouts/staff.html.erb
vi app/controllers/application_controller.rb

vi app/assets/stylesheets/satff/layout.css.scss
vi app/assets/stylesheets/staff/container.css.scss
vi app/assets/stylesheets/staff/_colors.css.scss
vi app/assets/stylesheets/staff/layout.css.scss
vi app/assets/stylesheets/staff/container.css.scss
vi app/assets/stylesheets/satff/_dimensions.css.scss
vi app/assets/stylesheets/staff/layout.css.scss
vi app/assets/stylesheets/staff/container.css.scss

vi config/secrets.yml
ruby -e 'require "securerandom"; print SecureRandom.hex(64)' > ~/.apptky_secret_key_base
export SECRET_KEY_BASE='cat ~/.apptky_secret_key_base'
vi config/database.yml
rails db:create RAILS_ENV=production

vi config/environments/production.rb
rails assets:precompile
rails s -e production


```


