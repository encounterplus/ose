{% if data.ac or data.aac -%}**{{'Common.AC'|l}}** {{data.ac}} \[{{data.aac}}\], {% endif -%}
{% if data.hd -%}**{{'Common.HD'|l}}** {{data.hd.value}}{{data.hd.mod|signed}}{% if data.hd.special %}{% for i in 1...data.hd.special %}*{% endfor %}{% endif %} {{data.hd.average|suffix: 'hp'|brackets}}, {% endif -%}
{% if data.attacks -%}**{{'Common.Att'|l}}** {{data.attacks}}, {% endif -%}
{% if data.thac0 or data.attackBonus -%}**{{'Common.THAC0'|l}}** {{data.thac0}} \[{{data.attackBonus|signed}}\], {% endif -%}
{% if data.movement -%}**{{'Common.MV'|l}}** {{data.movement}}, {% endif -%}
{% if true -%}
**{{'Monster.SV'|l}}** [{{'Saves.D'|l}}{{data.saves.death|default: 0}}](/roll/d20/death/save) [{{'Saves.W'|l}}{{data.saves.wands|default: 0}}](/roll/d20/wands/save) [{{'Saves.P'|l}}{{data.saves.paralysis|default: 0}}](/roll/d20/paralysis/save) [{{'Saves.B'|l}}{{data.saves.breath|default: 0}}](/roll/d20/breath/save) [{{'Saves.S'|l}}{{data.saves.spells|default: 0}}](/roll/d20/spells/save) {{data.saves.hd|brackets}}, {% endif -%}
{% if data.ml -%}**{{'Monster.ML'|l}}** {{data.ml}}, {% endif -%}
{% if data.alignment -%}**{{'Common.AL'|l}}** {{data.alignment|map: 'Alignment'}}, {% endif -%}
{% if data.xp -%}**{{'Common.XP'|l}}** {{data.xp}}, {% endif -%}
{% if data.na -%}**{{'Monster.NA'|l}}** {{data.na}}, {% endif -%}
{% if data.tt -%}**{{'Monster.TT'|l}}** {{data.tt}} {% endif -%}