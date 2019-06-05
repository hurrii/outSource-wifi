<template>
    <div class="news-pagination">
        <div class="btns-wrapper">
            <div class="btn-switchnews">
                <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M9 15L2 8L9 1" stroke="black" stroke-width="2"/>
                <path d="M16 8H2" stroke="black" stroke-width="2"/>
                </svg>


                <span>Предыдущая новость</span>
            </div>

            <div class="vertical-divider"></div>

            <div class="btn-switchnews">
                <span>Следующая новость</span>

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
                    height:80px
                }
            }

            .btn-switchnews {
                display: inline-block;
                width: 50%;
                text-align: center;

                &:hover {
                        svg path, span {
                        color: $pink;
                        stroke: $pink;
                    }
                }



                svg {
                vertical-align: top;

                    &:first-child { margin-right: 20px }
                    &:last-child { margin-left: 20px }
                }

            }
        }
</style>
