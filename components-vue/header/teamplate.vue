<template>
    <div class="frame">
      <div class="frame-wrapper">
        <div class="div">
          <Search class="huge-icon" color="#008AD2" />
          <div class="text-wrapper">Найти услугу</div>
        </div>
      </div>
      <div v-if="hasFrame" class="div-2">
        <img class="g" alt="G" src="g-10.png" />
        <div class="text-wrapper-2">Екатеринбургский медицинский центр</div>
      </div>
  
      <div class="div-3">
        <img class="img" alt="Frame" :src="frame" />
        <img class="line-2" alt="Line" :src="line" />
        <div class="div-4">
          <img class="huge-icon" alt="Huge icon" :src="hugeIcon" />
          <div class="div-5">
            <div class="text-wrapper-3">+7 (000) 000-00-00</div>
            <div class="text-wrapper">Единый телефон</div>
          </div>
        </div>
        <div class="div-6">
          <div class="text-wrapper-4">Обратный звонок</div>
          <img class="vector" alt="Vector" :src="vector" />
        </div>
      </div>
      <div class="vuesax-linear-user-wrapper">
        <IconComponentNode class="vuesax-linear-user" />
      </div>
      <div class="login-icons-wrapper">
        <div class="login-icons">
          <img class="vector-2" alt="Vector" :src="img" />
        </div>
      </div>
      <div class="div-7">
        <Menu
          class="menu-instance"
          :line="menuLine"
          :lineClassName="menuLineClassName"
          property1="frame-1597878956"
          text="О клинике"
        />
        <div class="div-8">
          <div class="text-wrapper-5">Отделения и услуги</div>
          <DirectionDown01 class="huge-icon-arrows" />
        </div>
        <div class="text-wrapper-5">Цены</div>
        <div class="text-wrapper-5">Специалисты</div>
        <div class="text-wrapper-5">Новости</div>
        <div class="text-wrapper-5">Вакансии</div>
        <div class="text-wrapper-5">Контакты</div>
        <div class="text-wrapper-5">Акции</div>
        <div class="text-wrapper-5">Информация</div>
      </div>
      <div class="div-9">
        <div v-if="hasDiv" class="div-10">
          <div class="group-wrapper">
            <div class="group">
              <div class="div-11">
                <img class="location" alt="Location" src="location-06.svg" />
                <div class="text-wrapper-6">Белореченская 23/1</div>
              </div>
            </div>
          </div>
          <div class="group-wrapper">
            <div class="div-wrapper">
              <div class="div-11">
                <img class="location" alt="Location" src="image.svg" />
                <div class="text-wrapper-6">Старых Большевиков 5</div>
              </div>
            </div>
          </div>
          <div class="group-wrapper">
            <div class="group-2">
              <div class="div-11">
                <img class="location" alt="Location" src="location-06-2.svg" />
                <div class="text-wrapper-6">Шевченко 9</div>
              </div>
            </div>
          </div>
          <div class="group-wrapper">
            <div class="group-3">
              <div class="div-11">
                <img class="location" alt="Location" src="location-06-3.svg" />
                <div class="text-wrapper-6">Родонитовая 10</div>
              </div>
            </div>
          </div>
        </div>
  
        <div :class="['group-wrapper-2', frameClassName]">
          <div class="group-4">
            <div class="div-11">
              <Time04 class="location" />
              <p class="text-wrapper-6">ПН-ПТ: с 8:00 до 20:00, СБ: с 9:00 до 18:00 | ВС: с 9:00 до 16:00</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import PropTypes from "prop-types";
  import { Search } from "./Search";
  import { IconComponentNode } from "./IconComponentNode";
  import { DirectionDown01 } from "./DirectionDown01";
  import { Time04 } from "./Time04";
  import { Menu } from "./Menu";
  
  export default {
    name: "Frame",
    components: {
      Search,
      IconComponentNode,
      DirectionDown01,
      Time04,
      Menu,
    },
    props: {
      hasFrame: {
        type: Boolean,
        default: true,
      },
      frame: {
        type: String,
        default: "frame-1597877825.svg",
      },
      line: {
        type: String,
        default: "line-13.svg",
      },
      hugeIcon: {
        type: String,
        default: "calling.svg",
      },
      vector: {
        type: String,
        default: "vector-339.svg",
      },
      img: {
        type: String,
        default: "vector.svg",
      },
      menuLine: {
        type: String,
        default: "line-40-3.svg",
      },
      hasDiv: {
        type: Boolean,
        default: true,
      },
      frameClassName: {
        type: String,
        default: "",
      },
    },
  };
  </script>
  
  <style>
  .frame {
    background-color: var(--white);
    border-bottom-style: solid;
    border-bottom-width: 1px;
    border-color: var(--border);
    height: 178px;
    overflow: hidden;
    position: relative;
    width: 1440px;
  }
  
  .frame .frame-wrapper {
    align-items: flex-start;
    border: 1px solid;
    border-color: var(--border);
    border-radius: 10px;
    display: inline-flex;
    flex-direction: column;
    gap: 10px;
    left: 349px;
    padding: 13px 143px 13px 15px;
    position: absolute;
    top: 56px;
  }
  
  .frame .div {
    align-items: center;
    display: inline-flex;
    flex: 0 0 auto;
    gap: 12px;
    justify-content: center;
    position: relative;
  }
  
  .frame .huge-icon {
    height: 22px !important;
    position: relative !important;
    width: 22px !important;
  }
  
  .frame .text-wrapper {
    color: var(--subtitle);
    font-family: "Onest-Regular", Helvetica;
    font-size: 14px;
    font-weight: 400;
    letter-spacing: 0;
    line-height: normal;
    position: relative;
    width: fit-content;
  }
  
  .frame .div-2 {
    align-items: center;
    display: inline-flex;
    gap: 14px;
    justify-content: center;
    left: 72px;
    position: absolute;
    top: 57px;
  }
  
  .frame .g {
    height: 46px;
    position: relative;
    width: 56px;
  }
  
  .frame .text-wrapper-2 {
    color: var(--blue);
    font-family: "Onest-Medium", Helvetica;
    font-size: 16px;
    font-weight: 500;
    letter-spacing: 0;
    line-height: normal;
    position: relative;
    width: 157px;
  }
  
  .frame .div-3 {
    align-items: center;
    display: inline-flex;
    gap: 20px;
    left: 670px;
    position: absolute;
    top: 56px;
  }
  
  .frame .img {
    flex: 0 0 auto;
    position: relative;
  }
  
  .frame .line-2 {
    height: 46px;
    object-fit: cover;
    position: relative;
    width: 1px;
  }
  
  .frame .div-4 {
    align-items: flex-start;
    display: inline-flex;
    flex: 0 0 auto;
    gap: 8px;
    position: relative;
  }
  
  .frame .div-5 {
    align-items: flex-end;
    display: inline-flex;
    flex: 0 0 auto;
    flex-direction: column;
    gap: 5px;
    position: relative;
  }
  
  .frame .text-wrapper-3 {
    color: var(--black);
    font-family: "Onest-Medium", Helvetica;
    font-size: 18px;
    font-weight: 500;
    letter-spacing: 0;
    line-height: normal;
    margin-top: -1px;
    position: relative;
    width: fit-content;
  }
  
  .frame .div-6 {
    align-items: center;
    background-color: var(--blue);
    border-radius: 10px;
    display: flex;
    gap: 10px;
    justify-content: center;
    padding: 14px 38px;
    position: relative;
    width: 220px;
  }
  
  .frame .text-wrapper-4 {
    color: var(--white);
    font-family: "Onest-Medium", Helvetica;
    font-size: 16px;
    font-weight: 500;
    letter-spacing: 0;
    line-height: 20.3px;
    margin-top: -1px;
    position: relative;
    white-space: nowrap;
    width: fit-content;
  }
  
  .frame .vector {
    height: 7px;
    left: 204px;
    position: absolute;
    top: 9px;
    width: 7px;
  }
  
  .frame .vuesax-linear-user-wrapper {
    border: 1px solid;
    border-color: var(--border);
    border-radius: 18px;
    height: 48px;
    left: 1320px;
    overflow: hidden;
    position: absolute;
    top: 56px;
    width: 48px;
  }
  
  .frame .login-icons-wrapper {
    border: 1px solid;
    border-color: var(--border);
    border-radius: 18px;
    height: 48px;
    left: 1262px;
    overflow: hidden;
    position: absolute;
    top: 56px;
    width: 48px;
  }
  
  .frame .login-icons {
    height: 24px;
    left: 12px;
    position: relative;
    top: 12px;
    width: 24px;
  }
  
  .frame .vector-2 {
    height: 16px;
    left: 1px;
    position: absolute;
    top: 4px;
    width: 22px;
  }
  
  .frame .div-7 {
    align-items: flex-start;
    display: inline-flex;
    gap: 67px;
    left: 72px;
    position: absolute;
    top: 134px;
  }
  
  .frame .menu-instance {
    flex: 0 0 auto !important;
  }
  
  .frame .div-8 {
    align-items: flex-start;
    display: inline-flex;
    flex: 0 0 auto;
    gap: 2px;
    position: relative;
  }
  
  .frame .text-wrapper-5 {
    color: var(--black);
    font-family: "Onest-Regular", Helvetica;
    font-size: 16px;
    font-weight: 400;
    letter-spacing: 0;
    line-height: normal;
    margin-top: -1px;
    position: relative;
    width: fit-content;
  }
  
  .frame .huge-icon-arrows {
    height: 20px !important;
    position: relative !important;
    width: 20px !important;
  }
  
  .frame .div-9 {
    background-color: var(--background);
    height: 36px;
    left: 0;
    position: absolute;
    top: 0;
    width: 1440px;
  }
  
  .frame .div-10 {
    align-items: flex-start;
    display: inline-flex;
    gap: 18px;
    left: 72px;
    position: absolute;
    top: 10px;
  }
  
  .frame .group-wrapper {
    align-items: flex-start;
    display: inline-flex;
    flex: 0 0 auto;
    gap: 30px;
    position: relative;
  }
  
  .frame .group {
    height: 17px;
    position: relative;
    width: 148px;
  }
  
  .frame .div-11 {
    align-items: center;
    display: inline-flex;
    gap: 6px;
    justify-content: center;
    position: relative;
  }
  
  .frame .location {
    height: 16px;
    position: relative;
    width: 16px;
  }
  
  .frame .text-wrapper-6 {
    color: var(--subtitle);
    font-family: "Onest-Regular", Helvetica;
    font-size: 13px;
    font-weight: 400;
    letter-spacing: 0;
    line-height: normal;
    margin-top: -1px;
    position: relative;
    width: fit-content;
  }
  
  .frame .div-wrapper {
    height: 17px;
    position: relative;
    width: 168px;
  }
  
  .frame .group-2 {
    height: 17px;
    position: relative;
    width: 97px;
  }
  
  .frame .group-3 {
    height: 17px;
    position: relative;
    width: 121px;
  }
  
  .frame .group-wrapper-2 {
    align-items: flex-start;
    display: inline-flex;
    gap: 30px;
    left: 942px;
    position: absolute;
    top: 10px;
  }
  
  .frame .group-4 {
    height: 17px;
    position: relative;
    width: 426px;
  }
  
  .frame .vuesax-linear-user {
    height: 22px !important;
    left: 13px !important;
    position: absolute !important;
    top: 13px !important;
    width: 22px !important;
  }
  </style>
  