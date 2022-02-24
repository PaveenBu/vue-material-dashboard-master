<template>
  <form>
    <md-card>
      <md-card-header :data-background-color="dataBackgroundColor">
        <h4 class="title">Form</h4>
        <p class="category">Complete your request form</p>
      </md-card-header>

      <md-card-content>
        <div class="md-layout">
          
          <div class="md-layout-item md-small-size-100 md-size-50">
            <md-field>
              <label>First Name</label>
              <md-input v-model="firstname" type="text"></md-input>
            </md-field>
          </div>
          <div class="md-layout-item md-small-size-100 md-size-50">
            <md-field>
              <label>Last Name</label>
              <md-input v-model="lastname" type="text"></md-input>
            </md-field>
          </div>
          <div class="md-layout-item md-small-size-100 md-size-100">
            <md-field>
              <label>Email Adress</label>
              <md-input v-model="address" type="text"></md-input>
            </md-field>
          </div>
          <div class="md-layout-item md-small-size-100 md-size-33">
            <md-field>
              <label>Action</label>
              <md-select v-model="action" name="action" id="action">
              <md-option value="Borrow">ยืม</md-option>
              <md-option value="Return">คืน</md-option>
              
          </md-select>
            </md-field>
          </div>
          <div class="md-layout-item md-small-size-100 md-size-33">
            <md-field>
              <label>Category</label>
                  <md-select v-model="category" name="category" id="category">
                  <md-option value="Computer">Computer</md-option>
                  <md-option value="Projector">Projector</md-option>
                  <md-option value="Networking Devices">Networking Devices</md-option>
                  <md-option value="Cable">Cable</md-option>
                </md-select>
            </md-field>
          </div>
          <div class="md-layout-item md-small-size-100 md-size-33">
            <md-field>
              <label>Assets</label>
              <md-input v-model="country" type="text"></md-input>
            </md-field>
          </div>
           <div>
            <md-datepicker v-model="selectedDate">
              <label>Select date</label>
            </md-datepicker>
          </div>
          <div class="md-layout-item md-size-100 text-right">
            <md-button class="md-raised md-success">SEND FORM</md-button>
          </div>
        </div>
      </md-card-content>
    </md-card>
  </form>
</template>
<script>
export default {
  name: "edit-profile-form",
  props: {
    dataBackgroundColor: {
      type: String,
      default: "",
    },
  
  },
  data() {
    return {
      emailadress: null,
      lastname: null,
      firstname: null,
      acton: null,
      category: null,
      assets: null,
      selectedDate: null,
      
    };
  },
};
</script>
<style></style>
