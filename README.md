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


```sh
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
vi app/controllers/admin/staff_members_controller.rb
vi app/controllers/admin/staff_members_controller.rb
vi app/views/admin/staff_members/new.html.erb
vi app/views/admin/staff_members/_form.html.erb
vi app/assets/stylesheets/admin/form.css.scss
vi app/controllers/admin/staff_members_controller.rb
vi app/views/admin/staff_members/edit.html.erb
vi app/views/admin/staff_members/_form_html.erb
vi app/controllers/admin/staff_members_controller.rb
vi config/application.rb
vi app/controllers/staff_members_controller.rb
vi app/controllers/admin/staff_members_controller.rb

vi app/application.rb
vi app/controllers/admin/staff_members_controller.rb
mkdir -p spec/controllers/admin
vi spec/controllers/admin/staff_members_controller_spec.rb
vi spec/factories/staff_members.rb
vi spec/controllers/admin/staff_members_controller_spec.rb
rails spec/controllers/admin/staff_members_controller_spec.rb
vi spec/controller/admin/staff_members_controller_spec.rb
rails spec/controllers/admin/staff_members_controller_spec.rb
vi app/controllers/concerns/errors_handlers.rb
vi app/views/errors/bad_request.html.erb
vi app/controllers/application_controller.rb
vi app/controllers/admin/staff_members_controller.rb

rails g controller staff/accounts
vi app/controllers/staff/accounts_controller.rb
vi app/views/shared/_header.html.erb
vi app/views/staff/accounts/show.html.erb
vi app/assets/stylesheets/layout.css.scss
vi app/assets/stylesheets/staff/tables.css.scss
vi app/controllers/staff/accounts_controller.rb
vi app/views/staff/acounts/edit.html.erb
vi app/views/staff/accounts/_form.html.erb
cp app/assets/stylesheets/admin/_form.html.scss app/assets/stylesheets/staff
vi app/controllers/staff/accounts_controller.rb
mkdir -p spec/controllers/staff
vi spec/controller/staff/accounts_controller_spec.rb
rails spec/controllers/staff/accounts_controller_spec.rb
vi spec/controllers/staff/accounts_controller_spec.rb
rails spec/controllers/staff/accounts_controller_spec.rb
vi app/controllers/admin/staff_members_controller.rb
vi app/controllers/admin/staff_members_controller.rb
vi app/controllers/admin/staff_members_controller.rb
vi app/controllers/admin/base.rb
vi app/controllers/admin/top_controller.rb
vi app/controllers/admin/sessions_controller.rb
vi app/controllers/staff/base.rb
vi app/controllers/staff/top_controller.rb
vi app/controllers/staff/sessions_controller.rb
vi app/controllers/staff_members.rb
vi app/controllers/staff/base.rb
vi app/controllers/staff/sessions_controller.rb
vi app/controllers/staff/base.rb
rails spec/
vi spec/controllers/admin/staff_members_controller_spec.rb
vi spec/controllers/staff/accounts_controller_spec.rb
rails spec/
mkdir -p spec/support
vi spec/support/shared_examples_for_admin_controllers.rb
vi spec/controllers/admin/staff-members_controller.spec.rb
vi spec/support/shared_examples_for_staff_controller.rb
vi spec/controllers/staff/accoutns_controller_spec.rb
rails spec/
vi spec/controller/staff/top_controller_spec.rb
vi spec/controller/staff/top_controller_spec.rb

vi Gemfile
bundle install
rails g model staff_event
rm spec/models/staff_event_spec.rb
vi db/migrate/202008010320_create_staff_events.rb
rails db:migrate
vi app/models/staff_member.rb
vi app/models/staff_event.rb
vi app/controllers/staff/sessions_controller.rb
// rails r "puts StaffMember.new.events.class.ancestors"
vi config/routes.rb
vi app/views/admin/top/dashboard.html.erb
curl https://localhost:3000/admin
vi app/views/admin/staff_members/index.html.erb

rails g controller admin/staff_events
vi app/controllers/admin/staff_events_controller.rb
vi app/views/admin/staff_events/index.html.erb
vi app/views/admin/staff_events/_event.html.erb
vi app/models/staff_event.rb
vi db/seeds.rb
vi db/seeds/development/staff_events.rb
rails db:reset
vi Gemfile
bundle install
rails g kaminari:config
rails g kaminari:views default
vi config/initializers/kaminari_config.rb
mkdir -p config/locales/views
vi config/locales/views/paginate.ja.yml
vi app/controllers/admin/staff_events_controller.rb
vi app/views/admin/staff_events/index.html.erb
vi app/views/kaminari/_paginator.html.erb
vi app/views/kaminari/_first_page.html.erb
vi app/views/kaminari/_last_page.html.erb
vi app/views/kaminari/_prev_page.html.erb
vi app/views/kaminari/_next_page.html.erb
vi app/assets/stylesheets/admin/pagination.css.scss
vi Gemfile
bundle install
vi app/controllers/admin/staff_events_controller.rb
vi app/controllers/admin/staff_controller.rb
vi app/app/controllers/admin/staff_event_controller.rb

vi Gemfile
bundle install
vi app/assets/stylesheets/admin/form.css.scss
vi app/assets/stylesheets/admin/_color.css.scss
vi app/models/staff_member.rb
vi app/models/concerns/string_normalizer.rb
vi app/models/staff_member.rb
vi app/models/staff_member.rb
vi app/models/concerns/string_normalizer.rb
vi app/models/staff_member.rb
vi app/models/staff_members.rb
vi app/models/staff_members.rb
vi spec/models/staff_members.rb
vi spec/models/staff_member_spec.rb
vi config/routes.rb
vi app/views/staff/acconts/show.html.erb
vi app/assets/stylesheets/tables.css.scss
rails g controller staff/passwords
vi app/controllers/staff/passwords.controller.rb
vi app/forms/change_password_form.rb
vi app/controllers/staff/password_controller.rb
vi app/views/staff/passwords/edit.html.erb

vi app/controllers/staff/passwords_controller.rb
vi app/forms/staff/change_password_form.rb
vi app/assets/stylesheets/form.css.scss
vi app/assets/stylesheets/staff/_color.css.scss
curl https://localhost:3000/password

vi app/views/admin/staff_members/index.html.erb
mkdir -p app/presenters
vi app/presenters/model_presenter.rb
vi app/presenters/staff_members_presenter.rb
vi app/views/admin/staff_members/index.html.erb
vi app/presenters/staff_memer_presenter.rb
vi app/views/staff_members/index.html.erb
vi app/presenters/model_presenter.rb
vi app/presenters/staff_member_presenter.rb
vi app/presenters/staff_member_presenter.rb
vi app/views/admin/staff_events/_event.html.erb
mkdir -p app/lib
app/lib/html_builder.rb
vi app/presenter/model_presenter.rb
vi app/presenters/staff_event_presenter.rb
vi app/views/admin/staff_events/index.html.erb
rm app/views/admin/staff_events/_event.html.erb
vi app/views/admin/staff_members/_form.html.erb
vi app/presenters/form_presenter.rb
vi app/presenters/staff_member_form_presenter.rb
vi app/views/admin/staff_members/_form.html.erb
vi app/assets/stylesheets/form.css.scss
vi app/presenters/staff_member_form_presenter.rb
vi app/presenters/form_presenter.rb
vi app/presenters/staff_member_form_presenter.rb
vi app/views/admin/staff_member/_form.html.erb
vi app/presenters/form_presenter.rb
vi app/presenters/staff_member_form_presenter.rb
vi app/helpers/application_helper.rb
vi app/views/admin/staff_members/_form.html.erb
vi app/views/admin/staff_members/_form.html.erb
mkdir -p config/locales/models
vi config/locales/modles/errors.ja.yml
vi config/locales/modles/staff_member.ja.yml
vi app/presenters/form_presenter.rb
vi app/presenters/form_presenter.rb
vi app/presenters/staff_member_form_presenter.rb
vi app/assets/stylesheets/admin/form.css.scss
curl https://localhost:3000/admin/staff_members/23
vi app/views/staff/passwords/edit.html.erb
mkdir -p config/locales/models/staff
vi config/locales/modle/staff/change_password_form.ja.yml
vi app/assets/stylesheets/staff/form.css.scss

vi app/assets/javascripts/application.js
vi app/assets/javascripts/application.js
cp app/assets/javascripts/application.js app/assets/javascripts/admin.js
cp app/assets/javascripts/application.js app/assets/javascripts/customer.js
cp app/assets/javascripts/application.js app/assets/staff.js
rm app/assets/javascripts/application.js
mkdir -p app/assets/javascripts/admin
mkdir -p app/assets/javascripts/customer
mkdir -p app/assets/javascripts/staff
mkdir -p app/assets/javascripts/shared

vi config/initializers/assets.rb
vi app/presenters/staff_member_form_presenter.rb
vi app/assets/javascripts/admin/staff_member_form.js.coffee
curl

vi Gemfile
bundle install
vi app/assets/javascripts/shared/datepicker.js.coffee
vi app/presenters/form_presenter.rb

rails g model customer
rails g model address
rm spec/models/customer_spec.rb
rm spec/models/address_spec.rb
vi db/migrate/202008011149_create_customer.rb
vi db/migrate/202008011149_create_addresses.rb
rails db:migrate
vi app/models/customer.rb
vi app/models/address.rb
vi app/models/home_addresses.rb
vi app/models/work_address.rb
vi db/seeds/development/customers.rb
vi db/seeds.rb
rails db:migrate
vi config/routes.rb
vi app/controllers/stafff/top_controller.rb
vi app/views/staff/top/dashboard.html.erb
vi spec/controllers/staff/top_controller_spec.rb
rails rspec
rails g controller staff/customers
vi app/controllers/staff/customers_controllers
vi app/controllers/staff/customers_controller.rb
vi app/presenters/customer_presenter.rb
vi app/views/staff/customers/index.html.erb
cp app/assets/stylesheets/admin/pagination.css.scss app/assets/stylesheets/staff
vi app/controllers/staff/customers_controller.rb
vi app/presenters/model_presenter.rb
vi app/presenters/address_presenter.rb
vi app/views/staff/customers/show.html.erb
vi app/views/staff/customer_form.rb
vi app/controllers/staff/customers_controller.rb
mv app/presenters/staff_member_form_presenter.rb app/presenters/
vi app/presenters/user_form_presenter.rb
vi app/presenters/staff_member_form_presenter.rb
vi app/presenters/customer_form_presenter.rb
vi app/presenters/address_form_presenter.rb
vi app/presenters/form_presenter.rb
vi app/views/staff/customers/new.html.erb
vi app/views/staff/customers/edit.html.erb
vi app/views/staff/customers/_form.html.erb
vi app/views/staff/customers/_customer_fields.html.erb
vi app/views/customers/_home_address_fields.html.erb
vi app/views/staff/customers/_work_address_fields.html.erb
cp app/assets/javascripts/admin/staff_member_form.js.coffee app/assets/javascripts/staff/customer_form.js.coffee
vi app/assets/javascripts/staff/customer_form.js.coffee
vi app/assets/javascripts/staff/datetimepicker.js.coffee
vi app/assets/stylesheets/shared/datepicker.css.scss

vi app/forms/staff/customer_form.rb
vi app/forms/staff/customer_form.rb
vi app/controllers/staff/customers_controller.rb
vi app/controllers/staff/customers_controller.rb

vi spec/support/features_spec_helper.rb
vi spec/factories/addresses.rb
vi spec/factories/customers.rb
mkdir -p spec/features/staff
spec/features/staff/customer_management_spec.rb
rails spec/features/staff/customer_management_spec.rb
rails spec/features/staff/customer_management_spec.rb
vi spec/features/staff/customer_management_spec.rb
rails spec/features/staff/customer_management_spec.rb
vi app/models/customer.rb
vi app/models/address.rb
vi app/models/concerns/string_normalizer.rb
vi app/models/home_address.rb
vi app/models/home_address.rb
vi app/models/work_address.rb
vi config/locales/models/customer.ja.yml
vi config/locales/models/address.ja.yml
vi app/forms/staff/customer_form.rb
vi app/forms/staff/customer_form.rb
vi app/forms/staff/customer_form.rb
vi app/forms/staff/customer_form.rb
vi spec/features/staff/customer_management_spec.rb
vi app/models/customer.rb
vi app/forms/staff/customer_form.rb
vi app/forms/customer_form.rb
vi app/models/staff_member.rb
vi app/models/concerns/personal_name_holder.rb
vi app/models/customer.rb
vi app/models/staff_member.rb
vi app/models/administrator.rb
vi app/models/concerns/email_holder.rb
vi app/models/customer.rb
vi app/models/administrator.rb
vi app/models/concerns/password_holder.rb
vi app/models/staff_member.rb
vi app/models/customer.rb
vi app/forms/staff/customer_form.rb
vi app/views/staff/customers/_form.html.erb

vi app/assets/javascripts/staff/customer_form.js.coffee
vi app/forms/staff/customer_form.rb
vi app/forms/staff/customer_form.rb
vi app/forms/staff/customer_form.rb
rails spec/features/staff/customer_manaement_spec.rb
vi spec/features/customer_management_spec.rb
rails spec/features/staff/customer_management_spec.rb
vi spec/features/staff/customer_management_spec.rb
rails spec/features/staff/customer_management_spec.rb
rails g model phone
rm spec/models/phone_spec.rb
vi db/migrate/202008011214_create_phones.rb
rails db:migrate
vi app/models/phone.rb
i app/models/concerns/string_normalizer.rb
vi app/models/customer.rb
vi app/models/address.rb
vi db/seeds/development/customers.rb
vi app/views/staff/customers/show.html.erb
vi app/presenters/customer_presenter.rb
vi app/presenters/address_presenter.rb
vi app/forms/staff/customer_form.rb
vi app/views/staff/customers/_customer_fields.html.erb

vi app/presenters/form_presenter.rb
vi app/views/staff/customers/_phone_fields.html.erb
vi app/forms/staff/customer_form.rb
vi spec/features/staff/phone_management_spec.rb
rails spec/features/staff/phone_management_spec.rb
vi app/forms/staff/customer_form.rb
vi app/views/staff/customers/_home_address_fields.html.erb
vi app/forms/staff/customer_form.html
vi spec/features/staff/phone_management_spec.rb
rails spec/features/staff/phone_management_spec.rb

rails g migration alter_customers1
rails g migration alter_addresses1
vi db/migrate/202008011219_alter_customers1.rb
vi db/migrate/202008011219_alter_addresses1.rb
rails db:migrate
vi app/models/customer.rb
vrails g migration update_customers1
vi db/migrate/202008011221_update_customers1.rb
rails db:migrate
rails db:rollback
rails db:migrate
vi app/forms/staff/customer_search_form.rb
vi app/controllers/staff/customers_controller.rb
vi app/views/staff/customers/_search_form.html.erb
vi app/views/staff/customers/index.html.erb
vi app/assets/stylesheets/staff/search.css.scss
vi app/controllers/staff/customer_controller.rb
vi app/forms/staff/customer_search_form.rb
vi app/forms/staff/customer_search_form.rb
vi app/models/customer.rb
vi app/models/customer.rb
vi app/forms/staff/customer_search_form.rb
```

---
---

```
vi config/routes.rb
vi config/environments/development.rb
vi app/controllers/staff/accounts_controller.rb
vi app/models/concerns/email_holder.rb
vi app/models/customer.rb
vi app/models/address.rb
vi app/models/concerns/string_normalizer.rb
vi app/assets/stylesheets/staff/flash.css.scss
vi app/assets/stylesheets/staff/_colors.css.scss
vi app/assets/stylesheets/staff/_dimensions.css.scss
vi app/assets/javascripts/admin/staff_member_form.js.coffee
vi app/forms/admin/login_form.rb
vi app/controllers/admin/sessions_controller.rb
vi app/views/admin/sessions/new.html.erb
vi app/services/admin/authenticator.rb
vi app/controllers/admin/sessions_controller.rb
vi app/presenters/customer_presenter.rb
vi app/presenters/model_presenter.rb
vi app/views/staff/customers/index.html.erb
vi app/lib/html_builder.rb
vi app/presenters/form_presenter.rb
vi app/views/admin/staff_members/_form.html.erb
vi spec/models/staff_member.rb
vi spec/factories/adminstrator.rb
vi app/controllers/admin/top_controller_spec.rb
vi spec/features/staff/phone_management_spec.rb

vi config/routes.rb
vi app/controllers/customer/base.rb
rails g controller customer/sessions
vi app/controllers/customer/sessions_controller.rb
vi app/controllers/customer/top_controller.rb
vi app/views/customer/sessions/new.html.erb
cp -f app/views/admin/shared/_header.html.erb app/views/customer/shared
vi app/views/customer/shared/_header.html.erb
vi app/forms/customer/login_form.rb
cp app/assets/stylesheets/admin/flash.css.scss app/assets/stylesheets/customer
cp app/assets/stylesheets/admin/session.css.scss app/assets/stylesheets/customer
vi app/assets/stylesheets/customer/sessions.css.scss
vi app/assets/stylesheets/customer/layout.css.scss
vi app/assets/stylesheets/customer/_colors.css.scss
mkdir -p app/services/customer
cp app/services/admin/authenticator.rb app/services/customer
vi app/services/customer/authenticator.rb
curl https://localhost:3000/mypage
vi app/forms/customer/login_form.rb
vi app/views/customer/sessions/new.html.erb
vi app/assets/stylesheets/customer/sessions.css.scss
vi app/controllers/customer/sessions_controller.rb
vi app/controllers/customer/session_controller.rb
vi app/controllers/customer/base.rb
mkdir -p spec/controllers/customer
vi spec/controllers/customer/sessions_controller_spec.rb
rails spec/controllers/customers/session_controller_spec.rb
vi spec/controllers/customer/sessions_controller_spec.rb
rails spec/controllers/customers/sessions_controller_spec.rb
vi config/environments/development.rb
vi app/controllers/application_controller.rb
vi app/controlllers/concerns/error_handlers.rb
rails g model AllowedSources
vi db/migrate/202008012312_create_allowed_sources.rb
rails db:migrate
vi app/models/allowed_source.rb
vi app/models/allowed_source.rb
vi spec/models/allowed_sources_spec.rb
rails spec/models/allowed_source_spec.rb
vi app/models/allowed_source.rb
vi spec/models/allowed_source_spec.rb
rails spec/models/allowed_source_spec.rb
rails spec
vi spec/rails_helper.rb
rails spec
vi app/models/allowed_source.rb
rails spec/models/allowed_source_spec.rb
vi app/controllers/staff/base.rb
vi spec/controllers/staff/top_controller_spec.rb
rails spec/controllers/staff/top_controller_spec.rb
curl https://localhost:3000/
rails r "AllowedSouurce.create(namespace: 'staff', ip_address: '10.0.2.2')"
vi config/environments/development.rb
vi config/routes.rb
vi app/views/admin/top/dashboard.html.erb
vi app/controllers/admin/allowed_sources_controller.rb
vi app/presenters/allowed_source_presenter.rb
vi app/views/admin/allowed_sources/index.html.erb
vi app/assets/stylesheets/admin/tables.css.scss
rails r "AllowedSource.create(namespace:'staff' ip_address:'127.0.0.1')"
rails r "AllowedSource.create(namespace:'staff', ip_address:'192.168.1.*')"
curl https://localhost:3000/admin/all
vi app/controllers/admin/allowed_sources_controller.rb
vi app/views/admin/allowed/sources/index.html.erb
vi app/views/admin/allowed_sources/_new_allowed_source.html.erb
vi app/models/allowed_source.rb
curl https://localhost:3000/admin/all
vi app/controllers/admin/allowed_sources_controller.rb
vi app/models/allowed_source.rb
vi app/views/admin/allowed_sources/index.html.erb
vi app/models/allowed_source.rb
vi app/services/admin/allowed_sources_deleter.rb
vi app/controllers/admin/allowed_sources_controller.rb
vi spec/controllers/admin/top_controller_spec.rb

rails g model program
rails g model entry
rm -rf spec/models/program_spec.rb
rm -rf spec/models/entry_spec.rb
vi db/migrate/202008012324_create_programs.rb
vi db/migrate/202008012324_create_entries.rb
rails db:migrate
vi app/models/entry.rb
vi app/models/program.rb
vi app/models/customer.rb
vi app/models/staff_member.rb
vi app/models/staff_member.rb
vi app/controllers/admin/staff_members_controllers.rb
vi db/seeds/development/programs.rb
vi db/seeds/development/entries.rb
vi db/seeds.rb
rails db:reset
vi config/routes.rb
vi app/views/staff/top/dashboard.html.erb
vi app/controllers/staff/programs_controller.rb
vi app/presenters/program_presenter.rb
vi app/views/staff/programs/index.html.erb
vi app/views/staff/programs/_program.html.erb
vi app/assets/stylesheets/staff/table.css.scss
vi app/controllers/staff/programs_controller.rb
vi app/views/staff/programs/show.html.erb
vi app/assets/stylesheets/staff/divs_and_spans.css.scss
vi spec/rails_helper.rb
rails spec
vi spec/support/performance_spec_helper.rb
spec/factories/programs.rb
vi spec/features/staff/program_management_spec.rb
rails -i performance spec/features/staff/program_management_spec.rb
cat log/performance_spec.log
vi app/controllers/staff/programs_controller.rb
rails -i performance spec/features/staff/program_management_spec.rb
vi app/models/program.rb
vi app/controllers/staff/programs_controller.rb
vi app/presenters/program_presenter.rb
vi app/presenters/program_presenter.rb
vi app/models/program.rb
vi app/presenters/program_presenter.rb
vi app/controllers/staff/programs_controller.rb
vi spec/features/staff/program_management-spec.rb
vi app/models/program.rb
vi app/models/program.rb
vi app/forms/staff/program_form.rb
vi app/controllers/staff/program_controller.rb
vi app/presenters/form_presenter.rb
vi app/presenters/program_form_presenter.rb
vi app/views/staff/programs/new.html.erb
vi app/views/staff/programs/eidt.html.erb
vi app/views/staff/programs/_form.html.erb
vi app/assets/stylesheets/staff/form.css.scss
vi app/controllers/staff/programs_controller.rb
vi app/forms/staff/program_form.rb
vi app/models/program.rb
curl https://localhost:30000/
vi app/lib/date_string_validator.rb
vi app/models/program.rb
vi config/locales/models/program.ja.yml
vi app/presenters/program_form_presenter.rb
vi app/assets/stylesheets/staff/form.css.scss
vi app/controllers/staff/programs_controller.rb
vi app/views/staff/programs/show.html.erb
vi app/views/staff/programs/_entries_form.html.erb
vi app/assets/stylesheets/staff/entries.css.scss
vi config/routes.rb
vi app/forms/staff/entries_form.rb
vi app/views/staff/programs/_entries_form.html.erb
vi app/views/staff/programs/_entries_form.html.erb
vi app/assets/javascripts/staff/entries_form.js.coffee
curl https://localhost:3000/programs/17
vi app/controllers/staff/programs_controller.rb
vi app/forms/staffentries_form.rb

```



