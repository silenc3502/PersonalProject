<template>
    <div>
        <h3>몬스터 도감 읽기</h3>
        <table>
            <tr>
                <td>몬스터번호</td>
                <td><input type="text" :value="monster.monsterNo" readonly></td>
            </tr>
            <tr>
                <td>등록일자</td>
                <td><input type="text" :value="monster.regDate" readonly></td>
            </tr>
            <tr>
                <td>몬스터명</td>
                <td><input type="text" :value="monster.name" readonly></td>
            </tr>
            <tr>
                <td>HP</td>
                <td><input type="number" :value="monster.hp" readonly></td>
            </tr>
            <tr>
                <td>경험치</td>
                <td><input type="number" :value="monster.exp" readonly></td>
            </tr>
            <tr>
                <td>드랍 머니</td>
                <td><input type="number" :value="monster.dropMoney" readonly></td>
            </tr>
            <tr>
                <td>드랍 아이템</td>
                <td><input type="text" :value="monster.dropItem" readonly></td>
            </tr>
            <tr>
                <td>몬스터 설명</td>
                <td><textarea cols="50" rows="15" :value="monster.description" readonly></textarea></td>
            </tr>
        </table>
    </div>
</template>

<script>

export default {
    name: 'MonsterRead',
    props: {
        monster: {
            type: Object,
            required: true
        }
    }    
}

</script>