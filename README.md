# lessons
https://laraveldaily.com/lesson/laravel-vue-inertia-food-delivery/restaurants-db-schema
# alias 
alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail'
# install breeze
https://laravel.com/docs/10.x/starter-kits#breeze-and-inertia
composer require laravel/breeze

php artisan breeze:install vue

# install ESlint
sail npm install --save-dev \
@rushstack/eslint-patch \
@vue/eslint-config-prettier \
eslint \
eslint-plugin-vue \
prettier

# Roles
admin- Администратор, управляет продавцами (владельцами ресторанов). Администратор создаст рестораны и учетные записи их владельцев.
vendor- Владелец ресторана может управлять меню ресторана и персоналом.
staff- Сотрудник принадлежит ресторану, управляется владельцем ресторана и выполняет заказы клиентов.
customer- Клиент может размещать заказы, а сотрудники обрабатывают заказы.admin- Администратор, управляет продавцами (владельцами ресторанов). Администратор создаст рестораны и учетные записи их владельцев.
vendor- Владелец ресторана может управлять меню ресторана и персоналом.
staff- Сотрудник принадлежит ресторану, управляется владельцем ресторана и выполняет заказы клиентов.
customer- Клиент может размещать заказы, а сотрудники обрабатывают заказы.

# create migration m m
php artisan make:migration create_role_user_table
