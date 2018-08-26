# Light card

light card is an light icon button for your light entities. 

The icon colors itself depending on the color of the light. If the color can not be detected (not supported by the light), a default warm yellow is used.

![light-card](light-1.png)

## Options

| Name | Type | Default | Description
| ---- | ---- | ------- | -----------
| type | string | **Required** | `custom:light-card`
| entity | string | **Required** | `light.office`
| icon | string | `mdi:lightbulb` | `mdi:desk-lamp`
| size | string | `40%` | Size of the icon. Can be percentage or pixel



## Examples


Import the card in `ui-lovelace.yaml` 
```yaml
title: Home
resources:
  - url: /local/light-card.js
    type: js
```

Show a light card for the office lights:
```yaml
- type: "custom:light-card"
  entity: light.office
  bulb_icon: mdi:desk-lamp
```
![light-card](office-light.png)


Show a light card with default bulb icon:
```yaml
- type: "custom:light-card"
  entity: light.desk_lamp
```
![light-card](desk-lamp.png)

