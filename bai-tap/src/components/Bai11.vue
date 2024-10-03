<template>
  <div class="container">
      <!-- Header start -->
      <v-container style="width: 300px;">
    <v-expansion-panels multiple="">
      <!-- Gender Section -->
      <v-expansion-panel>
        <v-expansion-panel-title>
            <template v-slot="">
            <span>Gender</span>
            </template>
        </v-expansion-panel-title>
        <v-expansion-panel-text>
            <v-radio-group>
                <v-radio label="Male" value="male"></v-radio>
                <v-radio label="Female" value="female"></v-radio>
            </v-radio-group>
        </v-expansion-panel-text>
        
      </v-expansion-panel>

      <!-- Categories Section -->
      <v-expansion-panel>
        <v-expansion-panel-title>
            <template v-slot="">
            <span>Categories</span>
            </template>
        </v-expansion-panel-title>
        <v-expansion-panel-text>
          <v-checkbox  label="All" value="all"></v-checkbox>
          <v-checkbox  label="Kitchen" value="kitchen"></v-checkbox>
          <v-checkbox  label="Electronics" value="electronics"></v-checkbox>
        </v-expansion-panel-text>
      </v-expansion-panel>

      <!-- Colors Section -->
      <v-expansion-panel>
        <v-expansion-panel-title>
            <template v-slot="">
            <span>Colors</span>
            </template>
        </v-expansion-panel-title>
        <v-expansion-panel-text>
          <v-checkbox  label="Green" value="all"></v-checkbox>
          <v-checkbox  label="Red" value="kitchen"></v-checkbox>
          <v-checkbox  label="Black" value="electronics"></v-checkbox>
        </v-expansion-panel-text>
      </v-expansion-panel>

      <!-- Price Section -->
      <v-expansion-panel>
        <v-expansion-panel-title>
            <template v-slot="">
            <span>Price</span>
            </template>
        </v-expansion-panel-title>
        <v-expansion-panel-text>
            <v-radio-group>
            <v-radio label="$10 - $50" value="10-50"></v-radio>
            <v-radio label="$50 - $100" value="50-100"></v-radio>
            <v-radio label="$100 - $150" value="100-150"></v-radio>
            <v-radio label="$150 - $200" value="150-200"></v-radio>
            <v-radio label="Over $200" value="over-200"></v-radio>
          </v-radio-group>
        </v-expansion-panel-text>
      </v-expansion-panel>

      <!-- Rating Section -->
      <v-expansion-panel>
        <v-expansion-panel-title>
            <template v-slot="">
            <span>Rating</span>
            </template>
        </v-expansion-panel-title>
        <v-expansion-panel-text>
            <v-rating length="5" color="yellow"></v-rating>
        </v-expansion-panel-text>
      </v-expansion-panel>
      <v-btn block color="primary" @click="resetFilters">
      Reset Filters
    </v-btn>
    </v-expansion-panels>

    <!-- Reset Filters Button -->
   
  </v-container>
       <!-- Header end -->
      <!-- Main start -->
       <v-container>
        <header style="display: flex;justify-content: space-between; align-items: center;">
            <div style="font-weight: 600;">Products</div>
            <div><v-text-field class="input" style="width: 250px;background-color: white;" label="Search" prepend-inner-icon="mdi-magnify">
                
            </v-text-field></div>
        </header>
        <div class="body-main">
            <v-card class="mx-auto"
            max-width="344">
            <v-img
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                cover
            ></v-img>
            <v-card-title>
            Top western road trips
            </v-card-title>
            <v-card-title style="display: flex;justify-content: space-between;">
                <div style="display: flex;gap: 5px;">
                   <h4 style="font-weight: 600;">15$</h4>
                   <p style="text-decoration: line-through;color: grey;font-size: smaller;">12$</p>
                </div>
               <div>
                <v-icon color="yellow">mdi-star</v-icon>
                <v-icon color="yellow">mdi-star</v-icon>
               </div>
            </v-card-title>
    
            </v-card>
            <v-card class="mx-auto"
            max-width="344">
            <v-img
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                cover
            ></v-img>
            <v-card-title>
            Top western road trips
            </v-card-title>
            <v-card-title style="display: flex;justify-content: space-between;">
                <div style="display: flex;gap: 5px;">
                   <h4 style="font-weight: 600;">15$</h4>
                   <p style="text-decoration: line-through;color: grey;font-size: smaller;">12$</p>
                </div>
               <div>
                <v-icon color="yellow">mdi-star</v-icon>
                <v-icon color="yellow">mdi-star</v-icon>
               </div>
            </v-card-title>
    
            </v-card>
            <v-card class="mx-auto"
            max-width="344">
            <v-img
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                cover
            ></v-img>
            <v-card-title>
            Top western road trips
            </v-card-title>
            <v-card-title style="display: flex;justify-content: space-between;">
                <div style="display: flex;gap: 5px;">
                   <h4 style="font-weight: 600;">15$</h4>
                   <p style="text-decoration: line-through;color: grey;font-size: smaller;">12$</p>
                </div>
               <div>
                <v-icon color="yellow">mdi-star</v-icon>
                <v-icon color="yellow">mdi-star</v-icon>
               </div>
            </v-card-title>
    
            </v-card>
            <v-card class="mx-auto"
            max-width="344">
            <v-img
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                cover
            ></v-img>
            <v-card-title>
            Top western road trips
            </v-card-title>
            <v-card-title style="display: flex;justify-content: space-between;">
                <div style="display: flex;gap: 5px;">
                   <h4 style="font-weight: 600;">15$</h4>
                   <p style="text-decoration: line-through;color: grey;font-size: smaller;">12$</p>
                </div>
               <div>
                <v-icon color="yellow">mdi-star</v-icon>
                <v-icon color="yellow">mdi-star</v-icon>
               </div>
            </v-card-title>
    
            </v-card>
            <v-card class="mx-auto"
            max-width="344">
            <v-img
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                cover
            ></v-img>
            <v-card-title>
            Top western road trips
            </v-card-title>
            <v-card-title style="display: flex;justify-content: space-between;">
                <div style="display: flex;gap: 5px;">
                   <h4 style="font-weight: 600;">15$</h4>
                   <p style="text-decoration: line-through;color: grey;font-size: smaller;">12$</p>
                </div>
               <div>
                <v-icon color="yellow">mdi-star</v-icon>
                <v-icon color="yellow">mdi-star</v-icon>
               </div>
            </v-card-title>
    
            </v-card>
            <v-card class="mx-auto"
            max-width="344">
            <v-img
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                cover
            ></v-img>
            <v-card-title>
            Top western road trips
            </v-card-title>
            <v-card-title style="display: flex;justify-content: space-between;">
                <div style="display: flex;gap: 5px;">
                   <h4 style="font-weight: 600;">15$</h4>
                   <p style="text-decoration: line-through;color: grey;font-size: smaller;">12$</p>
                </div>
               <div>
                <v-icon color="yellow">mdi-star</v-icon>
                <v-icon color="yellow">mdi-star</v-icon>
               </div>
            </v-card-title>
    
            </v-card>
            <v-card class="mx-auto"
            max-width="344">
            <v-img
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                cover
            ></v-img>
            <v-card-title>
            Top western road trips
            </v-card-title>
            <v-card-title style="display: flex;justify-content: space-between;">
                <div style="display: flex;gap: 5px;">
                   <h4 style="font-weight: 600;">15$</h4>
                   <p style="text-decoration: line-through;color: grey;font-size: smaller;">12$</p>
                </div>
               <div>
                <v-icon color="yellow">mdi-star</v-icon>
                <v-icon color="yellow">mdi-star</v-icon>
               </div>
            </v-card-title>
    
            </v-card>
            <v-card class="mx-auto"
            max-width="344">
            <v-img
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                cover
            ></v-img>
            <v-card-title>
            Top western road trips
            </v-card-title>
            <v-card-title style="display: flex;justify-content: space-between;">
                <div style="display: flex;gap: 5px;">
                   <h4 style="font-weight: 600;">15$</h4>
                   <p style="text-decoration: line-through;color: grey;font-size: smaller;">12$</p>
                </div>
               <div>
                <v-icon color="yellow">mdi-star</v-icon>
                <v-icon color="yellow">mdi-star</v-icon>
               </div>
            </v-card-title>
    
            </v-card>
        </div>
       </v-container>
       <!-- Main end -->
  </div>
</template>

<script setup>

</script>

<style scoped>
.container{
    display: flex;
    padding: 10px;
    border:2px solid rgb(207, 203, 203);
    border-radius: 5px;
}
.v-expansion-panel--active:not(:first-child), .v-expansion-panel--active + .v-expansion-panel {
    margin-top: 1px;
}
.v-field--variant-filled .v-field__overlay {
    background-color: white;
}
.v-field__loader{
    display: none;
}
.v-field__overlay {
    border: 1px solid red;
}
.body-main{
    display: grid;
    gap: 10px;
    grid-template-columns: auto auto auto auto;
}
</style>