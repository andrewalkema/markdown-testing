# markdown-testing

<pre><code>
output "clients" {
    value = concat(
    # If you have a single client registration, place it in this list
        [
            module.already_existing_service.data,
            <p color="green">module.my_service.data,</p>
            module.zz_existing_service.data,
        ],
    )
}
</code></pre>
