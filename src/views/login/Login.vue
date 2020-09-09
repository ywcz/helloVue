<template>
  <div>

    <b-row>
      <b-col
        md="6"
        offset-md="3"
      >
        <b-card>
          <b-form>
            <b-form-group
              id="input-group-1"
              label="UserName:"
              label-for="input-1"
            >
              <b-form-input
                id="input-1"
                v-model="user.name"
                type="text"
                required
                placeholder="Enter userName"
              ></b-form-input>
            </b-form-group>
            <b-form-group
              id="input-group-2"
              label="PhoneNumber:"
              label-for="input-2"
            >
              <b-form-input
                id="input-2"
                v-model="user.phoneNumber"
                type="text"
                required
                placeholder="Enter phoneNumber"
              ></b-form-input>
            </b-form-group>
            <b-form-group
              id="input-group-3"
              label="Password:"
              label-for="input-3"
            >
              <b-form-input
                id="input-3"
                v-model="user.password"
                type="password"
                required
                placeholder="Enter password"
              ></b-form-input>
            </b-form-group>
          </b-form>
        </b-card>
      </b-col>
    </b-row>

  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        name: '',
        phoneNumber: '',
        password: '',
      },
    };
  },
};
</script>
