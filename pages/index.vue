<template>
  <div id="app">
    <NonProtectedNavBar />
    <main>
        <Hero :heading="heroHeading" :btnLink="heroButtonLink" :btnText="heroButtonText"/>
        <Statistics :statistics="statistics"/>
        <HowItWorks :steps="hiwSteps" />
    </main>
  </div>
</template>

<script>
export default {
  data(){
    return {
      heroid: "hero",
      heroHeading: "Your Smart Personal Health Manager",
      heroButtonLink: "/login",
      heroButtonText: "Get Started",
      statisticsid: "statistics",
      statistics: [
        {
          id: 0,
          value: "40+",
          description: "Doctors Listed"
        },
        {
          id: 1,
          value: "100+",
          description: "Clients Registered"
        },
        {
          id: 2,
          value: "1k+",
          description: "Appointments Completed"
        },
        {
          id: 3,
          value: "10k+",
          description: "Medicine Reminders Sent"
        }
      ],
      howitworksid: "howitworks",
      hiwHeading: "How it works",
      hiwSteps: [
        {
          id: 0,
          image: require("~/assets/img/home/create.png"),
          value: "Create Your account",
          description: "Create an account to get started."
        },
        {
          id: 1,
          image: require("~/assets/img/home/add-content.png"),
          value: "Book your appointments",
          description: "Book Online Appointment with your Doctor."
        },
        {
          id: 2,
          image: require("~/assets/img/home/launch.png"),
          value: "Get Reminders",
          description: "Get reminders for your booked appointments/presciptions"
        }
      ]
    }
  }
};
</script>
