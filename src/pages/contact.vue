<template>
  <div
    class="q-table__container q-table--horizontal-separator column no-wrap q-table__card q-table--no-wrap no-shadow"
  >
    <div class="q-table__top relative-position row items-center">
      <div class="q-table__control">
        <div class="q-table__title">Contact Us</div>
      </div>
      <div class="q-table__separator col"></div>
      <div class="q-table__control">
        <label
          for="f_3d2cbd23-ffb3-42d3-a056-e259dc03cb11"
          class="q-field row no-wrap items-start q-input q-field--borderless q-field--dense q-validation-component"
          ><div class="q-field__inner relative-position col self-stretch">
            <div
              tabindex="-1"
              class="q-field__control relative-position row no-wrap"
            >
              <div
                class="q-field__control-container col relative-position row no-wrap q-anchor--skip"
              >
                <input
                  tabindex="0"
                  placeholder="Search"
                  id="f_3d2cbd23-ffb3-42d3-a056-e259dc03cb11"
                  type="text"
                  class="q-field__native q-placeholder"
                />
              </div>
              <div
                class="q-field__append q-field__marginal row no-wrap items-center"
              >
                <i
                  aria-hidden="true"
                  role="presentation"
                  class="material-icons q-icon notranslate"
                  >search</i
                >
              </div>
            </div>
          </div></label
        ><button
          tabindex="0"
          type="button"
          role="button"
          class="q-btn q-btn-item non-selectable no-outline q-px-sm q-btn--flat q-btn--round q-btn--actionable q-focusable q-hoverable q-btn--wrap q-btn--dense"
        >
          <span class="q-focus-helper"></span
          ><span class="q-btn__wrapper col row q-anchor--skip"
            ><span
              class="q-btn__content text-center col items-center q-anchor--skip justify-center row"
              ><i
                aria-hidden="true"
                role="img"
                class="material-icons q-icon notranslate"
                >fullscreen</i
              ><!----></span
            ></span
          ></button
        ><button
          tabindex="0"
          type="button"
          role="button"
          class="q-btn q-btn-item non-selectable no-outline q-btn--standard q-btn--rectangle bg-primary text-white q-btn--actionable q-focusable q-hoverable q-btn--no-uppercase q-btn--wrap"
        >
          <span class="q-focus-helper"></span
          ><span class="q-btn__wrapper col row q-anchor--skip"
            ><span
              class="q-btn__content text-center col items-center q-anchor--skip justify-center row"
              ><span class="block">Export to csv</span
              ><i
                aria-hidden="true"
                role="img"
                class="material-icons q-icon notranslate on-right"
                >archive</i
              ></span
            ></span
          >
        </button>
      </div>
    </div>
    <div class="q-table__middle scroll">
      <table class="q-table">
        <thead>
          <tr>
            <th class="text-left sortable">
              Division<i
                aria-hidden="true"
                role="presentation"
                class="q-table__sort-icon q-table__sort-icon--left material-icons q-icon notranslate"
                >arrow_upward</i
              >
            </th>
            <th class="text-left sortable">
              Email<i
                aria-hidden="true"
                role="presentation"
                class="q-table__sort-icon q-table__sort-icon--left material-icons q-icon notranslate"
                >arrow_upward</i
              >
            </th>
            <th class="text-left sortable">
              Postal Code<i
                aria-hidden="true"
                role="presentation"
                class="q-table__sort-icon q-table__sort-icon--left material-icons q-icon notranslate"
                >arrow_upward</i
              >
            </th>
            <th class="text-left sortable">
              Phone Number<i
                aria-hidden="true"
                role="presentation"
                class="q-table__sort-icon q-table__sort-icon--left material-icons q-icon notranslate"
                >arrow_upward</i
              >
            </th>
          </tr>
        </thead>
        <tbody>
          <tr class="">
            <td class="text-left">Management</td>
            <td class="text-left">
              <a target="__blank" href="business@gmail.com"
                >"business@gmail.com"</a
              >
            </td>
            <td class="text-left">5442645</td>
            <td class="text-left">+989391032885</td>
          </tr>
          <tr class="">
            <td class="text-left">Support</td>
            <td class="text-left">
              <a target="__blank" href="Support@gmail.com"
                >"Support@gmail.com"</a
              >
            </td>
            <td class="text-left">1336910</td>
            <td class="text-left">+989391091445</td>
          </tr>
          <tr class="">
            <td class="text-left">Delivery</td>
            <td class="text-left">
              <a target="__blank" href="Delivery@gmail.com"
                >"Delivery@gmail.com"</a
              >
            </td>
            <td class="text-left">2146910</td>
            <td class="text-left">+989391812445</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "contact",
});
</script>
