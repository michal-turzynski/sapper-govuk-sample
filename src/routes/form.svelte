<script>
  import { onMount } from "svelte";

  onMount(() => {
    console.log("mounting v2...");
    window.GOVUKFrontend.initAll();
  });
</script>

<style>
</style>

<svelte:head>
  <title>gov.uk | sample form</title>
</svelte:head>

<div class="govuk-warning-text">
  <span class="govuk-warning-text__icon" aria-hidden="true">!</span>
  <strong class="govuk-warning-text__text">
    <span class="govuk-warning-text__assistive">Warning</span>
    You can be fined up to £5,000 if you do not register.
  </strong>
</div>

<details class="govuk-details" data-module="govuk-details">
  <summary class="govuk-details__summary">
    <span class="govuk-details__summary-text">
      Help with nationality
    </span>
  </summary>
  <div class="govuk-details__text">
    We need to know your nationality so we can work out which elections you’re entitled to vote in. If you cannot provide your nationality, you’ll have to send copies of identity documents through the post.
  </div>
</details>

<fieldset class="govuk-fieldset">
  <legend class="govuk-fieldset__legend govuk-fieldset__legend--l">
    <h1 class="govuk-fieldset__heading">
      What is your address?
    </h1>
  </legend>

  <div class="govuk-form-group">
    <label class="govuk-label" for="address-line-1">
      Building and street <span class="govuk-visually-hidden">line 1 of 2</span>
    </label>
    <input class="govuk-input" id="address-line-1" name="address-line-1" type="text"></div>

  <div class="govuk-form-group">
    <label class="govuk-label" for="address-line-2">
      <span class="govuk-visually-hidden">Building and street line 2 of 2</span>
    </label>
    <input class="govuk-input" id="address-line-2" name="address-line-2" type="text"></div>

  <div class="govuk-form-group">
    <label class="govuk-label" for="address-town">
      Town or city
    </label>
    <input class="govuk-input govuk-!-width-two-thirds" id="address-town" name="address-town" type="text"></div>

  <div class="govuk-form-group">
    <label class="govuk-label" for="address-county">
      County
    </label>
    <input class="govuk-input govuk-!-width-two-thirds" id="address-county" name="address-county" type="text"></div>

  <div class="govuk-form-group">
    <label class="govuk-label" for="address-postcode">
      Postcode
    </label>
    <input class="govuk-input govuk-input--width-10" id="address-postcode" name="address-postcode" type="text"></div>
  
    <div class="govuk-character-count" data-module="govuk-character-count" data-maxlength="200">
      <div class="govuk-form-group">
        <label class="govuk-label" for="with-hint">
          Can you provide more detail?
        </label>
        <div id="with-hint-hint" class="govuk-hint">
          Do not include personal or financial information like your National Insurance number or credit card details.
        </div>
        <textarea class="govuk-textarea govuk-js-character-count" id="with-hint" name="with-hint" rows="5" aria-describedby="with-hint-info with-hint-hint"></textarea>
      </div>
    
      <div id="with-hint-info" class="govuk-hint govuk-character-count__message" aria-live="polite">
        You can enter up to 200 characters
      </div>
    
    </div>

</fieldset>
