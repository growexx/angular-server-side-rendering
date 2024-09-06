# Server Side Rendering with Angular

## Server-Side Rendering (SSR) with Angular involves using Angular Universal, a technology that allows Angular applications to be rendered on the server. This can improve the application's performance and SEO by serving the initial view of the page directly from the server.

### Here's how you can create a basic Angular SSR project and set up SSR with Angular Universal:

### 1. Install Angular CLI
    - Make sure we have Angular CLI installed globally. If we don’t have it, we can install it using:
    ```console
    npm install -g @angular/cli
    ```
### 2. Create a New Angular Project
    - Create a new Angular project by running:
    ```console
    ng new angular-server-side-rendering
    cd angular-server-side-rendering
    ```
### 3. Add Angular Universal to Your Project
    - We can add Angular Universal to our existing Angular project by running the following command:
    ```console
    ng add @nguniversal/express-engine
    ```
    - This command will configure our project for SSR, including adding the necessary server-side files and dependencies.
### 4. Build the Angular Application for SSR
    - After adding Angular Universal, we can build the application for SSR using:
    ```console
    npm run build:ssr
    ```
    - This will build the client and server bundles needed to run the application on the server.
### 5. Serve the Application on the Server
    - To serve our SSR-enabled Angular application, run:
    ```console
    npm run serve:ssr
    ```
    - This will start an Express server that serves our Angular application with SSR.
### 6. Test SSR
    - After running the server, open your browser and navigate to http://localhost:4000. You should see your Angular application, and if you inspect the page source, you’ll see that the HTML is fully rendered on the server side.
