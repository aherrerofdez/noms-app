<!-- src/routes/__layout.svelte -->
<script>
    export let menu;
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

    div {
        position: absolute;                 
        bottom: 0;
        margin-left: auto;
        margin-right: auto;
        left: 0;
        right: 0;
    }

    nav {
        display: flex;
        flex-direction: row;
        align-self: flex-end;
        border-top: solid #A2AAAE 1px;
    }

    a {
        display: flex;
        flex-direction: column;
        float: center;
        align-items: center;
        text-align: center;
        width: 20%;
        margin: 4px 12px;
        padding: 4px;
        text-decoration: none;
        color: #A2AAAE;
        font-family: 'Montserrat';
        font-size: 11px;
    }

    span {
        margin-top: 4px;
    }
</style>

<div>
    <nav>
        <a href="/" on:click={() => (menu = 1)}>
            {#if menu === 1}
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1"  width="24" height="24" viewBox="0 0 24 24">
                <path fill="#A2AAAE" d="M10,20V14H14V20H19V12H22L12,3L2,12H5V20H10Z" />
             </svg>
            {:else}
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1"  width="24" height="24" viewBox="0 0 24 24">
                <path fill="#A2AAAE" d="M12 5.69L17 10.19V18H15V12H9V18H7V10.19L12 5.69M12 3L2 12H5V20H11V14H13V20H19V12H22L12 3Z" />
            </svg>
            {/if}
            <span> Home </span>
        </a>
        <a href="/search" on:click={() => (menu = 2)}>
            {#if menu === 2}
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1"  width="24" height="24" viewBox="0 0 24 24">
                <path fill="#A2AAAE" d="M9.5,3C13.1,3,16,5.9,16,9.5c0,1.6-0.6,3.1-1.6,4.2l0.3,0.3h0.8l5,5L19,20.5l-5-5v-0.8l-0.3-0.3c-1.1,1-2.6,1.6-4.2,1.6
                    C5.9,16,3,13.1,3,9.5S5.9,3,9.5,3 M9.5,5C7,5,7.1,8.5,5,9.5c-2.3,1,2-5.2,4.5-5.2s6.7,6.4,4.5,5.2C11.4,8.1,12,5,9.5,5z"/>
            </svg>
            {:else}
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1"  width="24" height="24" viewBox="0 0 24 24">
                <path fill="#A2AAAE" d="M9.5,3A6.5,6.5 0 0,1 16,9.5C16,11.11 15.41,12.59 14.44,13.73L14.71,14H15.5L20.5,19L19,20.5L14,15.5V14.71L13.73,14.44C12.59,15.41 11.11,16 9.5,16A6.5,6.5 0 0,1 3,9.5A6.5,6.5 0 0,1 9.5,3M9.5,5C7,5 5,7 5,9.5C5,12 7,14 9.5,14C12,14 14,12 14,9.5C14,7 12,5 9.5,5Z" />
            </svg>
            {/if}
            <span> Search </span>
        </a>
        <a href="/series" on:click={() => (menu = 3)}>
            {#if menu === 3}
            <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 206.78 222.14">
                <style type="text/css">.main-color{fill: #a2aaae;} .white{fill: #fff;}</style>
                <g>
                    <circle class="main-color" cx="107.18" cy="122.54" r="99.6"/>
                    <ellipse class="main-color" cx="107.18" cy="121.97" rx="81.96" ry="80.52"/>
                    <ellipse class="main-color" cx="56.02" cy="51.3" rx="35.04" ry="40.8"/>
                    <ellipse class="main-color" cx="24.9" cy="88.86" rx="16.8" ry="14.64"/>
                    <ellipse class="white" cx="865.47" cy="457.18" rx="15.56" ry="16.8" transform="translate(-707.61 736.11) rotate(-70)"/>
                    <rect class="white" x="848.31" y="468.91" width="10.42" height="7.9" transform="translate(-696 -582.77) rotate(15)"/>
                    <ellipse class="main-color" cx="101.22" cy="38.08" rx="25.44" ry="18.62"/>
                    <ellipse class="white" cx="941.29" cy="403.77" rx="20.91" ry="25.5" transform="translate(-669.92 708.25) rotate(-65)"/>
                    <ellipse class="white" cx="894.91" cy="418.66" rx="36.35" ry="40.8" transform="translate(-906.57 -216.22) rotate(-10)"/>
                </g>
            </svg>
            {:else}
            <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 206.78 222.14">
                <style type="text/css"> .main-color{fill: #a2aaae;} .white{fill: #fff;}</style>
                <g>
                    <circle class="main-color" cx="107.18" cy="122.54" r="99.6"/>
                    <ellipse class="white" cx="107.18" cy="121.97" rx="81.96" ry="80.52"/>
                    <ellipse class="main-color" cx="56.02" cy="51.3" rx="35.04" ry="40.8"/>
                    <ellipse class="main-color" cx="24.9" cy="88.86" rx="16.8" ry="14.64"/>
                    <ellipse class="white" cx="865.47" cy="457.18" rx="15.56" ry="16.8" transform="translate(-707.61 736.11) rotate(-70)"/>
                    <rect class="white" x="848.31" y="468.91" width="10.42" height="7.9" transform="translate(-696 -582.77) rotate(15)"/>
                    <ellipse class="main-color" cx="101.22" cy="38.08" rx="25.44" ry="18.62"/>
                    <ellipse class="white" cx="941.29" cy="403.77" rx="20.91" ry="25.5" transform="translate(-669.92 708.25) rotate(-65)"/>
                    <ellipse class="white" cx="894.91" cy="418.66" rx="36.35" ry="40.8" transform="translate(-906.57 -216.22) rotate(-10)"/>
                </g>
            </svg>
            {/if}
            <span> Series </span>
        </a>
        <a href="/bundles" on:click={() => (menu = 4)}>
            {#if menu === 4}
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1"  width="24" height="24" viewBox="0 0 24 24">
                <path fill="#A2AAAE" d="M17,18C15.89,18 15,18.89 15,20A2,2 0 0,0 17,22A2,2 0 0,0 19,20C19,18.89 18.1,18 17,18M1,2V4H3L6.6,11.59L5.24,14.04C5.09,14.32 5,14.65 5,15A2,2 0 0,0 7,17H19V15H7.42A0.25,0.25 0 0,1 7.17,14.75C7.17,14.7 7.18,14.66 7.2,14.63L8.1,13H15.55C16.3,13 16.96,12.58 17.3,11.97L20.88,5.5C20.95,5.34 21,5.17 21,5A1,1 0 0,0 20,4H5.21L4.27,2M7,18C5.89,18 5,18.89 5,20A2,2 0 0,0 7,22A2,2 0 0,0 9,20C9,18.89 8.1,18 7,18Z" />
            </svg>
            {:else}
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1"  width="24" height="24" viewBox="0 0 24 24">
                <path fill="#A2AAAE" d="M17,18A2,2 0 0,1 19,20A2,2 0 0,1 17,22C15.89,22 15,21.1 15,20C15,18.89 15.89,18 17,18M1,2H4.27L5.21,4H20A1,1 0 0,1 21,5C21,5.17 20.95,5.34 20.88,5.5L17.3,11.97C16.96,12.58 16.3,13 15.55,13H8.1L7.2,14.63L7.17,14.75A0.25,0.25 0 0,0 7.42,15H19V17H7C5.89,17 5,16.1 5,15C5,14.65 5.09,14.32 5.24,14.04L6.6,11.59L3,4H1V2M7,18A2,2 0 0,1 9,20A2,2 0 0,1 7,22C5.89,22 5,21.1 5,20C5,18.89 5.89,18 7,18M16,11L18.78,6H6.14L8.5,11H16Z" />
            </svg>
            {/if}
            <span> Bundles</span>
        </a>
        <a href="/info" on:click={() => (menu = 5)}>
            {#if menu === 5}
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1"  width="24" height="24" viewBox="0 0 24 24">
                <path fill="#A2AAAE" d="M13,9H11V7H13M13,17H11V11H13M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2Z" />
             </svg>
            {:else}
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1"  width="24" height="24" viewBox="0 0 24 24">
                <path fill="#A2AAAE" d="M11,9H13V7H11M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M11,17H13V11H11V17Z" />
            </svg>
            {/if}
            <span> Info </span>
        </a>
    </nav>
</div>

<slot></slot>