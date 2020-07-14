<template>


    <div>
        <div class="container">


            <div class="row mb-4">
                <div class="col-12">
                    <div class="card">
                        <div class="card-body">
                            <chart></chart>

                        </div>

                    </div>

                </div>
            </div>
            <div class="row mb-4">

                <div class="col-3">
                    <user1 :baslik=" 'Current Online' " :deger=" ' 0' "></user1>


                </div>
                <div class="col-3">
                    <user1 :baslik=" 'Max Online' " :deger=" ' 1' "></user1>

                </div>
                <div class="col-3">
                    <user1 :baslik=" 'Unique     Connections' " :deger=" ' 3' "></user1>

                </div>
                <div class="col-3">
                    <user1 :baslik=" 'Impresions' " :deger=" ' 42' "></user1>

                </div>
            </div>

            <div class="row mb-4">
                <div class="col-6">
                    <div class="card">
                        <div class="card-body">
                            <donut-chart></donut-chart>
                        </div>
                    </div>
                </div>
                <div class="col-6">
                    <div class="card">
                        <div class="card-body">
                            <donut-chart></donut-chart>

                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <user-detail></user-detail>
                <user-edit></user-edit>

            </div>
        </div>


    </div>

</template>
<script>

    import User1 from "@/components/User1";
    import Chart from "@/components/Chart";
    import DonutChart from "@/components/DonutChart";
    import UserDetail from "@/components/UserDetail";
    import UserEdit from "@/components/UserEdit";


    export default {
        name: 'HelloWorld',
        components: {
            UserEdit,
            UserDetail,

            User1,
            Chart,
            DonutChart


        },


        methods: {
            handler() {
                var args = arguments;
                for (var arg of args) {
                    if (arg instanceof Function) {
                        arg();
                    }
                }
            }
        },
        computed: {}


    }
</script>
<style>
    div.container {
        margin-top: 30px;
        padding: 20px 40px;
        background-color: rgba(186, 183, 183, 0.17);
        border: 1px solid #a7b0b1;

    }
</style>

