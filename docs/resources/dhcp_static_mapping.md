---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "pfsense_dhcp_static_mapping Resource - terraform-provider-pfsense"
subcategory: ""
description: |-
  IPv4 DHCP Static Mapping
---

# pfsense_dhcp_static_mapping (Resource)

IPv4 DHCP Static Mapping



<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `interface` (String) Interface to assign this static mapping to. You may specify either the interface's descriptive name, the pfSense interface ID (e.g. wan, lan, optx), or the real interface ID (e.g. igb0).
- `mac` (String) MAC address of the host this mapping will apply to.

### Optional

- `arp_table_static_entry` (Boolean) Create a static ARP entry for this static mapping.
- `client_identifier` (String) Set a client identifier.
- `description` (String) Description for this mapping
- `dns_servers` (List of String) DNS servers to assign this client. Each value must be a valid IPv4 address.
- `domain` (String) Domain for this host.
- `domain_search_list` (List of String) Search domains to assign to this host. Each value be a valid domain name.
- `gateway` (String) Gateway to assign this host. This value must be a valid IPv4 address within the interface's subnet.
- `host_name` (String) Hostname for this host.
- `ip_address` (String) IPv4 address the MAC address will be assigned.

### Read-Only

- `id` (String) The ID of this resource.