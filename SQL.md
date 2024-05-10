Comando Ler Agua GERAL




```shell

SELECT  MSG_ID, MSG_ENTITY, SUBSTRING(MSG_JSON, position('volume_2' in MSG_JSON)+10, 4) WATER FROM `tbl_export` WHERE MSG_ENTITY = 'zigbee2mqtt/water_geral' order by MSG_ID desc

```
