<script setup lang="ts"></script>

<template>
  <input type="file" name="picture" id="picture">
  <div class="card_pablic">
    <div class="pin_title">

    </div>

    <div class="pin_modal">
        <div class="modal_head">
            <div class="save_card">Save</div>
        </div>
        <div class="modal_foot">
            <div class="destination">
                <div class="pint_mock_icon_container">
                    <img src="@/components/images/top-right.png" alt="Место назначения" class="pint_mock_icon">
                </div>
                <span>Eatery</span>
            </div>
            <div class="pint_mock_icon_container">
                    <img src="@/components/images/send.png" alt="Отправить" class="pint_mock_icon">
            </div>
            <div class="pint_mock_icon_container">
                    <img src="@/components/images/more.png" alt="Редактироввть" class="pint_mock_icon">
            </div>
        </div>
    </div>

    <div class="pin_image">
        <img src="" alt="Изображение">
    </div>
  </div>
</template>

<style>
    .card_pablic {
        width: 236px;
        height: 472px;
        background-color: rgb(128, 132, 148);
        border-radius: 16px;
        position: relative;
        overflow: hidden;
    }
    .pin_title {
        width: 0px;
        padding: 0px;
        opacity: 0;
    }
    .pin_modal {
        width: 100%;
        height: 100%;
        position: absolute;
        background-color: rgba(0, 0, 0, 0.1);
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        opacity: 1; /* в конце вернуть на 0 */
        transition-duration: 0.3s;
        z-index: 9999;
    }
    .pin_modal:hover {
        opacity: 1;
    }
    .pin_modal .modal_head {
        width: 100%;
        height: 15%;
        position: fixed;
        top: 0;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }
</style>