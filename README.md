<style>
            .social-btn-element{
                display: flex;
                justify-content: center;
                padding: 1%;
            }

            .social-btn,a{
                background: rgb(255, 255, 255); /* สีพื้นหลังของปุ่ม */
                color: rgb(0, 0, 0); /* สีตัวอักษร  */
                transition: all .4s ease; /* อนิเมชั่นปุ่มลอยมึงลองปรับเล่นๆดู เเต่กูว่า 4 กำลังดี */
                border-radius: 12px; /* โค้งมนของปุ่ม */
                padding: 12px; /* ระยะห่างรอบนอก ซ้ายบนขวาล่าง ทำให้เว้นสวยงาม*/
                margin: 1.6px; /* ระยะห่างรอบใน ซ้ายบนขวาล่าง ทำให้เว้นสวยงาม */
                width: 10%; /* ความยาวของปุ่ม ปล. ที่ตั้งเเบบนี้เพราะให้มปุ่มมันยาวเท่ากันเเละสม่ำเสมอกัน */
                height: 100%; /* อันนี้คือความสูงความกว้าง 100% = ให้ความอิสระของความใหญ่ยาวปุ่ม */
                text-decoration: none; /* เอาเส้นใต้ตัวอักษรออก */
            }

            .social-btn:hover{ /* ทั้งหมดนี้เป็นส่วนของ อนิเมชั่นเเอกชั่นของปุ่ม okป่ะ ไอตรงที่เป็นเงา 3 ชั้นอ่ะ */
                transform: translate(-12px, -12px);
            }
            .social-btn:hover::after{
                transform: translate(6px, 6px);
            }
            .social-btn:hover::before{
                transform: translate(12px, 12px);
            }

            .social-btn::after,.social-btn::before{ /* ตรงนี้ก็เป็น อนิเมชั่นเเอกชั่นของปุ่ม okป่ะ ไอตรงที่เป็นเงา 3 ชั้นอ่ะ 
                                                            เเต่ตรงนี้จะเป็นตัวกำหนดลักษณะตกเเต่งอีกที เช่น สี ความสูงความใหญ่ 100% */
                content: '';
                position: absolute;
                opacity: .3;
                background: rgb(255, 255, 255); /* สีเงา ปล ถ้าเปลี่ยนต้องเป็นสีเดียวกันกับ สีพื้นหลังปุ่มนะ สีพื้นหลังอยู่นี่ >> .social-btn,a */
                border-radius: inherit;
                width: 100%;
                height: 100%;
                left: 0px;
                bottom: 0px;
                z-index: -1;
                transition: all .25s ease;
            }
        </style>
