{%p if jurisdiction_type == “siac” %}
This Agreement shall be governed by the SIAC Rules.
{%p endif %}

Parties:
{%p for party in parties_list %}
- {{ party.name }}, incorporated in {{ party.place_of_incorporation }}
{%p endfor %}

This Agreement is governed by {{ country_name(governing_law) }}.
