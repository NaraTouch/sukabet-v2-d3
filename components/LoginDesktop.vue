<template>
    <form class="form-inline">
        <div class="form-check mr-sm-2">
            <label class="form-check-label">
                Lupa Password?
            </label>
        </div>
        <div class="input-group mr-sm-2">
            <div class="input-group-prepend">
                <div class="input-group-text">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-person-fill" viewBox="0 0 16 16">
                        <path d="M3 14s-1 0-1-1 1-4 6-4 6 3 6 4-1 1-1 1H3zm5-6a3 3 0 1 0 0-6 3 3 0 0 0 0 6z"/>
                    </svg>
                </div>
            </div>
            <input type="text" class="form-control"  placeholder="Login ID">
        </div>
        <div class="input-group mr-sm-2">
            <div class="input-group-prepend">
                <div class="input-group-text">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-lock" viewBox="0 0 16 16">
                        <path d="M8 1a2 2 0 0 1 2 2v4H6V3a2 2 0 0 1 2-2zm3 6V3a3 3 0 0 0-6 0v4a2 2 0 0 0-2 2v5a2 2 0 0 0 2 2h6a2 2 0 0 0 2-2V9a2 2 0 0 0-2-2zM5 8h6a1 1 0 0 1 1 1v5a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1V9a1 1 0 0 1 1-1z"/>
                    </svg>
                </div>
            </div>
            <input type="password" class="form-control" placeholder="Password">
        </div>
        <div class="input-group mr-sm-2">
            <button class="btn-theme btn-red no-border" type="submit">Masuk</button>
        </div>
        <div class="input-group mr-sm-2">
            <button class="btn-theme btn-white no-border" type="submit">Daftar</button>
        </div>
    </form>
</template>