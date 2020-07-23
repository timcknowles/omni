<template>
  <v-card>
    <v-tabs
     fixed-tabs
      v-model="tab"
      background-color="purple darken-4"
      dark
    >
      <v-tab
        v-for="item in items"
        :key="item.tab"
      >
        {{ item.tab }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
        
      >
        <div class="tab-item-wrapper">
            <v-card flat>
            <v-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis viverra, elit vel tempus fringilla, velit ex ullamcorper libero, sit amet aliquam felis tellus quis mauris. Curabitur a diam nec enim porttitor scelerisque eget vitae leo. Curabitur nec enim id velit gravida consectetur. Integer eu nulla bibendum, pulvinar est eu, semper nunc. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Vivamus molestie urna lacus, ac suscipit risus suscipit nec. Sed pretium augue mi, eget congue sapien volutpat et. Aenean mattis nulla dapibus dolor efficitur condimentum. Interdum et malesuada fames ac ante ipsum primis in faucibus. Nunc dolor metus, blandit id ultrices vel, condimentum ut urna. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. In nisi mauris, tristique eu porttitor non, condimentum ac nisl.

In tristique bibendum velit. Donec placerat accumsan eros quis rutrum. Etiam elit tellus, pulvinar in ex eget, tempor viverra magna. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Donec congue leo sit amet sem efficitur consequat. Nulla elit neque, laoreet lacinia velit et, suscipit varius ante. Nulla quis nisi sed dui aliquam iaculis. Maecenas ac purus ac purus tempor maximus. Maecenas volutpat ante erat, in tempor mi bibendum id. Nulla dictum tempus nisl ac venenatis. Nunc quis urna convallis, cursus orci eu, convallis erat. Praesent et libero urna. Aenean vehicula maximus dolor, et cursus mi. Sed varius lobortis ex, vitae ullamcorper eros volutpat et.</v-card-text>
            </v-card>
          
        </div>
      </v-tab-item>
      <v-tab-item
        
      >
        <div class="tab-item-wrapper">
            <v-card flat>
            <v-card-text><Dose /></v-card-text>
            </v-card>
          
        </div>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
  
</template>

<script>
  export default {
    data () {
      return {
        tab: null,
        items: [
          { tab: 'Setup', content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis viverra, elit vel tempus fringilla, velit ex ullamcorper libero, sit amet aliquam felis tellus quis mauris. Curabitur a diam nec enim porttitor scelerisque eget vitae leo. Curabitur nec enim id velit gravida consectetur. Integer eu nulla bibendum, pulvinar est eu, semper nunc. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Vivamus molestie urna lacus, ac suscipit risus suscipit nec. Sed pretium augue mi, eget congue sapien volutpat et. Aenean mattis nulla dapibus dolor efficitur condimentum. Interdum et malesuada fames ac ante ipsum primis in faucibus. Nunc dolor metus, blandit id ultrices vel, condimentum ut urna. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. In nisi mauris, tristique eu porttitor non, condimentum ac nis' },
          { tab: 'Dose Adjustment', content: '<Calcium />'},
        //   { tab: 'Three', content: 'Tab 3 Content' },
        //   { tab: 'Four', content: 'Tab 4 Content' },
        //   { tab: 'Five', content: 'Tab 5 Content' },
        //   { tab: 'Six', content: 'Tab 6 Content' },
        //   { tab: 'Seven', content: 'Tab 7 Content' },
        //   { tab: 'Eight', content: 'Tab 8 Content' },
        //   { tab: 'Nine', content: 'Tab 9 Content' },
        //   { tab: 'Ten', content: 'Tab 10 Content' },
        ],
      }
    },
  }
</script>

<style>
    .tab-item-wrapper {
    /* vuetify sets the v-tabs__container height to 48px */
    height: calc(100vh - 48px);
    width: calc(100vh - 48px);

    }
    
</style>