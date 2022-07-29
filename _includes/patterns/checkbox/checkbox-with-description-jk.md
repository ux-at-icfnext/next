
<form class="usa-form">
  <fieldset class="usa-fieldset">
    <legend class="usa-legend">Select any {{page.topic | downcase}}</legend>
    {% assign category = page.topic | downcase | replace: ' ', '-' %}
    {% for item in page.checkbox %}
    {% assign value = item.title | downcase | replace: ' ', '-' %}
    <div class="usa-checkbox">
      <input
        class="usa-checkbox__input usa-checkbox__input--tile"
        id="check-{{value}}"
        type="checkbox"
        name="{{category}}"
        value="{{value}}"
      />
      <label class="usa-checkbox__label" for="check-{{value}}">
        {{item.title}}
        <span class="usa-checkbox__label-description">
            {{item.description}}
        </span>
        </label>
    </div>
    {% endfor %}
  </fieldset>
</form>