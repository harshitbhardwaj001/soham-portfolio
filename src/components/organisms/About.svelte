<script>
import RichPresence from '../molecules/RichPresence.svelte';
import Tooltip from '../atoms/Tooltip.svelte';

// i didnt write this idk
let getAge = () => {
    let birthDate = new Date('2004/08/14');
    const ageMs = Date.now() - birthDate.getTime();
    const preciseAge = (ageMs / 31536000000).toFixed(10);
    return preciseAge;
};

let age = getAge();
setInterval(() => {
    age = getAge();
}, 1000);
</script>

<section id="about" class="wrapper">
    <div>
        <RichPresence />
    </div>
    <div class="text">
        <h2>bio</h2>
        <p>
            Hey there, I'm Soham! :] I'm a <Tooltip tip={age}
                ><span>{Math.floor(Number(age))}</span></Tooltip
                >
                year old digital artist and graphic/UI designer based in Mumbai. I’ve taken art seriously since
                <span>2017</span>, and have been doodling 3D art work since <span>2020</span>.
                Recently, however, I've grown a knack for video editing. I like contributing my services to
                <Tooltip tip="🤓">
                    <a href="https://github.com/xafn" target="_blank" rel="noreferrer">
                        <span>events</span>
                    </a>
                </Tooltip>
                as a designer, which is probably the reason why you've ended up here. Currently working on building my digital marketplace <Tooltip tip="🤓">
                    <a href="https://www.studiodzns.com/" target="_blank" rel="noreferrer">
                        <span>DZNS</span>
                    </a>
                </Tooltip>.
                </p>
                </div>
                </section>

<style lang="scss">
@import '../../styles/mixins.scss';

section {
    margin-bottom: 6rem;
    display: grid;
    gap: 4.5rem;
    grid-template-columns: 1fr 1fr;
    align-items: center;
}

.text {
    position: relative;
    line-height: 1.75rem;
}

span {
    font-weight: 400;
    font-family: var(--font-two);
    font-size: 0.9rem;
    background-color: var(--elevation-one);
    border-radius: 7px;
    color: var(--accent);
    padding: 0.2rem 0.5rem 0.2rem;
    width: fit-content;
}

a {
    text-decoration: none;
}

.text::before {
    @include outlineText($content: 'dzns',
        $translateX: 27%,
        $translateY: -2%,
        $fontSize: 300px,
        $opacity: 0.22);
}

h2 {
    display: none;
    margin-top: 1rem;
}

@media (max-width: 868px) {
    section {
        display: flex;
        flex-direction: column;
        align-items: normal;
    }

    h2 {
        display: block;
        margin-bottom: 1rem;
    }
}
</style>
