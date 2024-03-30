
**{{'Class.Requirements'|l}}:** {% if data.requirements %}{{data.requirements}}{% else %}{{'Common.None'|l}}{% endif %}
**{{'Class.PrimeRequisite'|l}}:** {% if data.primeRequisite %}{{data.primeRequisite}}{% else %}{{'Common.None'|l}}{% endif %}
**{{'Class.HitDice'|l}}:** {% if data.hd %}1d{{data.hd}}{% else %}{{'Common.None'|l}}{% endif %}
**{{'Class.MaximumLevel'|l}}:** {{data.maximum|default: 0}}
**{{'Class.Armour'|l}}:** {% if data.armour %}1d{{data.armour}}{% else %}{{'Common.None'|l}}{% endif %}
**{{'Class.Weapons'|l}}:** {% if data.weapons %}1d{{data.weapons}}{% else %}{{'Common.None'|l}}{% endif %}
**{{'Class.Languages'|l}}:** {% if data.languages %}{{data.languages| map: 'Language'}}{% else %}{{'Common.None'|l}}{% endif %}