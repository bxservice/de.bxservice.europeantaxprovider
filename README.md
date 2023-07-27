# de.bxservice.europeantaxprovider

In the European Union, there is a regulation that the tax applied to an order is based on the shipping address rather than the invoice address. However, when creating a Sales Order in iDempiere, the tax is set by default based on the bill address.

This plugin addresses the issue by adjusting the tax calculation for both Sales and Purchase Orders. It ensures that the correct tax is applied by setting the appropriate invoice address before calling the Core method.

To utilize this plugin, simply install it on your server and configure the System with the TAX_LOOKUP_SERVICE set to 'de.bxservice.europeantaxprovider.BXSTaxLookup'.
