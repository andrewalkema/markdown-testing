```hcl
output "clients" {
	value = concat(
		# If you have a single client registration, place it in this list
		[
			module.already_existing_service.data,
			<strong>module.my_service.data,</strong>
			module.zz_existing_service.data,
		],
	)
}
```
