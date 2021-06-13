<script context='module'>
    export function getDate(){
        let newDate = new Date();
        return `${newDate.getDay()}/${newDate.getMonth()}/${newDate.getFullYear()}`
    }
</script>