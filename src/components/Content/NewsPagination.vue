<template>
    <div class="news-pagination">
        <div class="btns-wrapper">
            <div class="chevron">
                <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M9 15L2 8L9 1" stroke="black" stroke-width="2"/>
                <path d="M16 8H2" stroke="black" stroke-width="2"/>
                </svg>
            </div>
            <div class="btn-switchnews">
                Предыдущая новость
            </div>

            <div class="vertical-divider"></div>

            <div class="btn-switchnews">Следующая новость
            </div>
            <div class="chevron">
                <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M7 1L14 8L7 15" stroke="black" stroke-width="2"/>
                <path d="M0 8H14" stroke="black" stroke-width="2"/>
                </svg>
            </div>
        </div>
    </div>
</template>

<script>

export default {
  name: 'NewsPagination'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
        .news-pagination {
            width: 100%;
            background: #F4F4F4;
            height: 80px;

                @media screen and (min-width: 1024px) { height: 120px; }
            
                    display: flex;
                    align-items: center;

            .btns-wrapper {
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    width: 100%;
                    cursor: pointer;

                .vertical-divider {
                    border-left:1px solid rgba(0, 0, 0, 0.1);
                    height: 80px
                }
            }

            .btn-switchnews {
                font-size: 14px;
                text-align: center;
                max-width: 40%;
                flex: 1;

                @media screen and (min-width: 768px) { font-size: 18px; }
                @media screen and (min-width: 1024px) { font-size: 20px; }
            
            }


            svg {
              @media screen and (max-width: 580px) {
              width: 10px;
              height: 10px;
            }
        }
    }
</style>
