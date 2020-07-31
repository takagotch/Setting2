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

```
vi config/environments/production.rb
vi app/controllers/staff/top_controller.rb
rails s -e production
curl https://localhost:3000/staff
vi app/controllers/application_controller.rb
mkdir -p app/views/errors
vi app/views/errors/internal_server_error.html.erb
vi app/assets/stylesheets/errors.css.scss
vi app/assets/stylesheets/admin.css
vi app/assets/stylesheets/customer.css
rails assets:precompile RAILS_ENV=production
vi app/controllers/application_controller.rb
vi app/views/errors/forbidden.html.erb
vi app/controllers/admin/top_controller.rb
curl https://localhost:3000/admin
vi app/controllers/customer/top_controller.rb
vi config/routes.rb
rails g controller errors
vi app/controllers/errors_controller.rb
vi app/controllers/application_controller.rb
vi app/views/not_found.html.erb
curl https://localhost:3000/errors
vi app/controllers/application_controller.rb
vi app/controllers/customer/top_controller.rb
curl https://localhost:3000/customer
vi app/controllers/application_controller.rb
vi app/controllers/concerns/error_handlers.rb
vi app/controllers/application_controller.rb
vi app/controllers/application_controller.rb
vi config/environments/production.rb
```

```
rails g model StaffMember
vi db/migrate/202008010232_create_staff_members.rb
vi db/migrate/202008010232_create_staff_members.rb
rails db:migrate
// rails r 'StaffMember.columns.each { |c| p [ c.name, c.type ]}'
vi app/models/staff_member.rb
vi app/models/staff_member.rb
vi spec/models/staff_member_spec.rb
vi spec/models/staff_member_spec.rb
vi spec/models/staff_member_spec.rb
rails spec/models/staff_member_spec.rb
vi db/seeds.rb
mkdir -p db/seeds/development
vi db/seeds/development/staff_members.rb
rails db:seed
rails db:reset

rails r 'puts StaffMember.count'
rails r 'puts StaffMember.first.hashed_password'

vi app/controller/staff/base.rb
vi app/controllers/staff/top_controller.rb
vi confit/routes.rb
mkdir app/views/staff/shared
mkdir app/views/admin/shared
mkdir app/views/customer/shared
cp app/views/shared/_header.html.erb app/views/staff/shared/
cp app/views/shared/_header.html.erb app/views/admin/shared/
cp app/views/shared/_header.html.erb app/views/customer/shared/
rm app/views/shared/_header.html.erb

vi app/views/layouts/staff.html.erb
vi app/views/layouts/admin.html.erb
vi app/views/layouts/customer.html.erb
vi app/views/staff/shared/_header.html.erb
vi app/assets/stylesheets/staff/layout.css.scss

mkdir -p app/forms/staff
vi app/forms/staff/login_form.rb
rails g controller staff/sessions
vi app/controllers/staff/sessions_controller.rb
vi app/views/staff/sessions/new.html.erb
vi app/controllers/sessions_controller.rb
curl https://localhost:3000/staff/login
vi app/controllers/staff/sessions_controller.rb
vi app/assets/stylesheets/staff/sessions.css.scss
mkdir -p app/services/staff
vi app/services/staff/authenticator.rb
vi app/controllers/staff/sessions_controller.rb
mkdir spec/factories
vi spec/factories/staff_members.rb
mkdir -p spec/services/staff
vi spec/services/staff/authenticator_spec.rb
rails spec/services/staff/authenticator_spec.rb
vi app/controllers/staff/sessions_controller.rb
app/views/staff/shared/_header.html.erb
vi app/assets/stylesheets/staff/flash.css.scss
vi app/assets/stylesheets/staff/_color.css.scss
curl https://localhost:3000/staff/session

vi config/routes.rb
vi config/routes.rb
vi config/routes.rb
curl https://localhost:3000/

vi config/routes.rb
vi Rails.application.routes.draw do
vi config/routes.rb
app/controller/admin/top_controller.rb
vi app/views/admin/top/dashboard.html.erb
curl https://localhost:3000/admin
vi config/routes.rb
vi config/routes.rb
vi config/routes.rb
curl https://localhost:3000/
curl https://localhost:3000/admin
vi config/environments/development.rb
vi config/routes.rb
vi config/routes.rb
vi config/routes.rb
curl https://localhost:3000/
curl https://localhost:3000/admin
mkdir spec/routing
vi spec/routing/hostname_constraints_spec.rb
vi spec/routing/hostname_constraints_spec.rb

rails g controller admin/staff_members
vi db/development/staff_members.rb
rails db:reset
vi app/controllers/admin/staff_members_controller.rb
vi app/views/amin/staff_members/index.html.erb
vi app/assets/stylesheets/admin/tables.css.scss
vi app/views/admin/_header.html.erb
vi app/assets/stylesheets/admin/layout.css.scss


```

