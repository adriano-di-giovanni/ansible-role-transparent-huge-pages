# Ansible Role: Transparent Huge Pages

Ansible role to disable transparent huge pages

## Requirements

Ansible 2.x

## Role variables

<table>
  <thead>
    <tr>
      <th>variable</th>
      <th>required</th>
      <th>default</th>
      <th>choices</th>
      <th>comment</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>thp_x_start_before</td>
      <td>no</td>
      <td>[]</td>
      <td>&nbsp;</td>
      <td>This service will start before the services listed here</td>
    </tr>
  </tbody>
</table>

## Dependencies

None.

## Example playbook

```YAML
---
- hosts: all
  become: true
  roles:
    - role: adriano-di-giovanni.ansible-role-transparent-huge-pages
      thp_x_start_before:
        - redis
        - mongod
```

## License

MIT

## Author information

Adriano Di Giovanni
