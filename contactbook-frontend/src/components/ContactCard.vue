<script>
export default {
    props: {
        contact: { type: Object, required: true },
    },
};
</script>
<template>
    <div>
        <div class="p-1">
            <strong>Tên:</strong>
            {{ contact.name }}

        </div>
        <div class="p-1">
            <strong>E-mail:</strong>
            {{ contact.email }}
        </div>
        <div class="p-1">
            <strong>Địa Chỉ:</strong>
            {{ contact.address }}
        </div>
        <div class="p-1">
            <strong>Điện Thoại:</strong>
            {{ contact.phone }}
        </div>
        <div class="p-1">
            <strong>Favorite:&nbsp;</strong>
            <i v-if="contact.favorite" class="fas fa-check" />
            <i v-else class="fas fa-times" />
        </div>
    </div>
</template>