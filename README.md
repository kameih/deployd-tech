<div class="container">
          <h1>API end Points:</h1>
          <ul>
            <li><a href="#">http://127.0.0.1:8000/api/register</a></li>
            <li><a href="#">http://127.0.0.1:8000/api/login</a></li>
            <li><a href="#">http://127.0.0.1:8000/api/get_user</a></li>
          </ul>
        </div>

        <div class="entry-content blog-details wp-block-post-content is-layout-constrained wp-block-post-content-is-layout-constrained"> 

            <h2 class="wp-block-heading nitro-offscreen nitro-lazy-render" id="16-step-1-install-laravel">Step 1. Install laravel</h2> <p class="nitro-offscreen nitro-lazy-render"><strong>composer create-project laravel/laravel (name any suitable app name)</strong></p> 

            <h2 class="wp-block-heading nitro-offscreen nitro-lazy-render" id="17-step-2-install-jwt-package">Step 2. Install JWT Package And NPM package</h2> <pre class="wp-block-code nitro-offscreen nitro-lazy-render"><code>composer require tymon/jwt-auth</code></pre> <pre class="wp-block-code nitro-offscreen nitro-lazy-render"><code>npm install</code></pre> 


         <h2 class="wp-block-heading nitro-offscreen nitro-lazy-render" id="19-step-4-publish-jwt-configuration">Step 3. Publish jwt configuration</h2> <pre class="wp-block-code nitro-offscreen nitro-lazy-render"><code>php artisan vendor:publish --provider="Tymon\JWTAuth\Providers\LaravelServiceProvider"</code></pre> 

         <h2 class="wp-block-heading nitro-offscreen nitro-lazy-render" id="20-step-5-generate-jwt-key">Step 4. Generate JWT Key</h2> <p class="nitro-offscreen nitro-lazy-render"><strong>Command</strong>:</p> <pre class="wp-block-code nitro-offscreen nitro-lazy-render"><code>php artisan jwt:secret</code></pre> 


         <h2 class="wp-block-heading nitro-offscreen nitro-lazy-render" id="21-step-6-create-jwt-middleware">Step 5. Create jwt middleware</h2> <p class="nitro-offscreen nitro-lazy-render">Command: php artisan make:middleware JwtMiddleware</p>   

         <h2 class="wp-block-heading nitro-offscreen nitro-lazy-render" id="22-step-7-configure-database">Step 6. Configure database</h2>   <p> <pre>
              DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=test_rest_api_db
DB_USERNAME=root
DB_PASSWORD=
         </pre>
            

         </p>

         <h2 class="wp-block-heading nitro-offscreen nitro-lazy-render" id="24-step-9-create-api-controller">Step 7. Create api controller</h2> <p class="nitro-offscreen nitro-lazy-render"><strong>Create API controller<br><br></strong>Create a JWTAuthController controller.</p> <pre class="wp-block-code nitro-offscreen nitro-lazy-render"><code>php artisan make:controller ApiController</code></pre> <p class="nitro-offscreen nitro-lazy-render">This command will create the fresh new controller here: <strong>app\Http\Controllers\ApiController.php</strong></p> 




<h2 class="wp-block-heading nitro-offscreen nitro-lazy-render" id="31-step-16-migrate-database">Step 8: Migrate database</h2> <p class="nitro-offscreen nitro-lazy-render"><strong>Command:</strong></p> <pre class="wp-block-code nitro-offscreen nitro-lazy-render"><code>php artisan migrate</code></pre>


 <h2 class="wp-block-heading nitro-offscreen nitro-lazy-render" id="32-step-17-now-start-the-development-server">Step 9. Now start the development server</h2> <p class="nitro-offscreen nitro-lazy-render"><strong>Command</strong>:</p> <pre class="wp-block-code nitro-offscreen nitro-lazy-render"><code>php artisan serve</code></pre> 

