<template>
    <div id="burger-table">
        <div>
            <div id="burger-table-heading">
                <div class="order-id">#:</div>
                <div>Cliente:</div>
                <div>Pao:</div>
                <div>Carne:</div>
                <div>Opcionis:</div>
                <div>Ações:</div>
                <!-- <div>Status:</div> -->
            </div>
        </div>
        <div id="burger-table-rows">
            <div class="burger-table-row">
                <div class="order-number">1</div>
                <div>Zezim</div>
                <div>Pão 3 queijos</div>
                <div>Maminha</div>
                <div>
                    <ul>
                        <li>Salame</li>
                        <li>Tomate</li>
                    </ul>
                </div>
                <div>
                    <select name="status" class="status">
                        <option value="">Selecione </option>
                    </select>
                    <button id="delete-btn">Cancelar</button>
                </div>
            </div>
            <div class="burger-table-row">
                <div class="order-number">1</div>
                <div>Zezim</div>
                <div>Pão 3 queijos</div>
                <div>Maminha</div>
                <div>
                    <ul>
                        <li>Salame</li>
                        <li>Tomate</li>
                    </ul>
                </div>
                <div>
                    <select name="status" class="status">
                        <option value="">Selecione </option>
                    </select>
                    <button id="delete-btn">Cancelar</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
#burger-table{
    max-width: 1200px;
    margin: 0 auto;
}

#burger-table-heading,
#burger-table-rows,
.burger-table-row{
    display: flex;
    flex-wrap: wrap;
}
#burger-table-heading{
    font-weight: bold;
    padding: 10px;
    border-bottom: 3px solid #333;

}

#burger-table-heading div,
.burger-table-row div{
    width: 19%;
}

.burger-table-row{
    width: 100%;
    padding: 12px;
    border-bottom: 1px solid #ccc ;

}

#burger-table-heading .order-id,
.burger-table-row .order-number{
    width: 4%;
}

select{
    padding: 12px 6px;
    margin-right: 12px ;
}

#delete-btn{
    background-color: #222;
    color:#fcba03 ;
    font-weight: bold;
    border: 2px solid #222;
    padding: 10px;
    font-size: 16px;
    /* margin: 0px auto; */
    cursor: pointer;
    transition: .5s;
}

#delete-btn:hover{
    background-color: transparent ;
    color: #222;
}

</style>