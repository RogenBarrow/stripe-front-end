<!-- src/routes/+layout.svelte -->
<script>
    import '../app.css';
</script>

<!-- Main Layout Structure -->
<div
    class="bg-cover bg-center bg-no-repeat h-screen bg-gradient-to-b"
    style="background-image: url('/background.png');"
>
    <header>
        <nav class="px-8 py-4 w-full min-w-[320px] font-sans">
            <div class="container mx-auto flex items-center justify-between">
                <!-- Centered navigation links (including "Stripe" logo) -->
                <div class="flex mx-auto items-center justify-center space-x-8">
                    <!-- "Stripe" logo (always visible) -->
                    <svg
                        viewBox=" 0 0 120 60"
                        xmlns="http://www.w3.org/2000/svg"
                        width="80"
                        height="60"
                        fill-rule="evenodd"
                        fill="white"
                        ><path
                            d="M101.547 30.94c0-5.885-2.85-10.53-8.3-10.53-5.47 0-8.782 4.644-8.782 10.483 0 6.92 3.908 10.414 9.517 10.414 2.736 0 4.805-.62 6.368-1.494v-4.598c-1.563.782-3.356 1.264-5.632 1.264-2.23 0-4.207-.782-4.46-3.494h11.24c0-.3.046-1.494.046-2.046zM90.2 28.757c0-2.598 1.586-3.678 3.035-3.678 1.402 0 2.897 1.08 2.897 3.678zm-14.597-8.345c-2.253 0-3.7 1.057-4.506 1.793l-.3-1.425H65.73v26.805l5.747-1.218.023-6.506c.828.598 2.046 1.448 4.07 1.448 4.115 0 7.862-3.3 7.862-10.598-.023-6.667-3.816-10.3-7.84-10.3zm-1.38 15.84c-1.356 0-2.16-.483-2.713-1.08l-.023-8.53c.598-.667 1.425-1.126 2.736-1.126 2.092 0 3.54 2.345 3.54 5.356 0 3.08-1.425 5.38-3.54 5.38zm-16.4-17.196l5.77-1.24V13.15l-5.77 1.218zm0 1.747h5.77v20.115h-5.77zm-6.185 1.7l-.368-1.7h-4.966V40.92h5.747V27.286c1.356-1.77 3.655-1.448 4.368-1.195v-5.287c-.736-.276-3.425-.782-4.782 1.7zm-11.494-6.7L34.535 17l-.023 18.414c0 3.402 2.552 5.908 5.954 5.908 1.885 0 3.264-.345 4.023-.76v-4.667c-.736.3-4.368 1.356-4.368-2.046V25.7h4.368v-4.897h-4.37zm-15.54 10.828c0-.897.736-1.24 1.954-1.24a12.85 12.85 0 0 1 5.7 1.47V21.47c-1.908-.76-3.793-1.057-5.7-1.057-4.667 0-7.77 2.437-7.77 6.506 0 6.345 8.736 5.333 8.736 8.07 0 1.057-.92 1.402-2.207 1.402-1.908 0-4.345-.782-6.276-1.84v5.47c2.138.92 4.3 1.3 6.276 1.3 4.782 0 8.07-2.368 8.07-6.483-.023-6.85-8.782-5.632-8.782-8.207z"
                        /></svg
                    >

                    <!-- Main navigation links (hidden on small screens, visible on md and larger screens) -->
                    <div class="hidden md:flex space-x-8">
                        <a class="text-white" href="/about">Products</a>
                        <a class="text-white" href="/services">Solutions</a>
                        <a class="text-white" href="/contact">Developers</a>
                        <a class="text-white" href="/dashboard">Resources</a>
                        <a class="text-white" href="/pricing">Prices</a>
                    </div>
                </div>

                <!-- Right-aligned actions (hidden on small screens, visible on md and larger screens) -->
                <div class="hidden md:flex space-x-6">
                    <a class="text-white" href="/signin">Sign in</a>
                    <button class="rounded-full bg-white px-4"
                        >Contact Sales</button
                    >
                </div>
            </div>
        </nav>
    </header>

    <main>
        <aside>
            <!-- Sidebar content (e.g., additional navigation or user info) -->
        </aside>

        <section>
            <slot />
        </section>
    </main>
</div>

<footer>
    <!-- Footer content (e.g., copyright, contact info) -->
</footer>
